
## Пример запроса

```
https://sqs.mcs.mail.ru/123456789012/MyQueue/
?Action=TagQueue
&Tag.Key=QueueType
&Tag.Value=Production
&Expires=2020-10-18T22:52:43PST
&Version=2012-11-05
&AUTHPARAMS
```

## Пример ответа

```
<TagQueueResponse>
   <ResponseMetadata>
      <RequestId>a1b2c3d4-e567-8901-23f4-g5678901hi23</RequestId>
   </ResponseMetadata>
</TagQueueResponse>
```