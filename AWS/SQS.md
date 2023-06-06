#### **Simple Queue Service**
If we are receiving data from external source and we want to process them but when the data comes in bulk and we cannot process it in the same rate then we can push the extra data or events to the queue and when the server is free then it will pop the message data one by one and process it.

SQS can **subscribe** topics then will be published by [[SNS]]. 
