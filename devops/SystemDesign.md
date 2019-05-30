# AWS System Design

Please design a multi-region AWS architecture for a server 
application with the following requirements. Architecture 
you will design should consist of AWS resources and their 
relationships. Assume you will be presenting this architecture 
to your colleagues and you will discuss strength and weaknesses
of it. We encourage you to use drawings. Most of the time, 
a diagram can tell more than thousands of words.

Please keep the design as simple as possible with only 
necessary resources. We would not expect you to spend more
than three hours on it.

**Requirements:**
* Application will expose an API to be used by third parties. No need to worry about front-end.
* API will be consumed in the US and Europe.
* There will be endpoints for uploading and downloading media. We will need a media storage.
* There will be user membership. We need some sort of database to keep information related to members.
* You may assume average read/write ratio of API services will be 10/1 (read-heavy).
* Load may go up to 1k RPS at the peak and go down to 1 RPS at the idle. We need something to scale up and down without manual intervention.
