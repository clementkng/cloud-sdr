### Patch oddness:
```
patches/0001-1st-msg-hub-go-example-working.patch:52: trailing whitespace.
*/
patches/0001-1st-msg-hub-go-example-working.patch:142: trailing whitespace.
*/
warning: 2 lines add whitespace errors

```

### Tests (but don't try to hard given these are old commits):
Hard given no available MSGHUB_API_KEY. I also can’t verify the brokerUrls are still up (but probably not because “bluemix” is in the URL). I tried creating a new key w/ Event Streams (the closest IBM cloud service I could find to the old message hub), and also tried an old key I had at hand but just got timeout errors when I attempted the messages in the Readme. I attempted the commands again with my own generated certificates, but given that the original certificate is supposed to last 10 years if I’m reading the keys correctly (365 days/year * 10), this isn’t working. 
Starting message hub publishing example...
[sarama] 2022/04/10 23:15:59 Initializing new client
[sarama] 2022/04/10 23:15:59 client/metadata fetching metadata for all topics from broker kafka04-prod02.messagehub.services.us-south.bluemix.net:9093
[sarama] 2022/04/10 23:16:29 Failed to connect to broker kafka04-prod02.messagehub.services.us-south.bluemix.net:9093: dial tcp 169.60.0.119:9093: i/o timeout
[sarama] 2022/04/10 23:16:29 client/metadata got error from broker -1 while fetching metadata: dial tcp 169.60.0.119:9093: i/o timeout

### Other observations:
This introduces 2 msghub providers, meant to publish messages to IBM Message hub. One using confluent kafka and the other doesn’t. Peeking ahead, it looks like the one using confluent kafka will not work nor be supported.
The certificates are not supposed to be here. They get removed later.
