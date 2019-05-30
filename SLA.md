# Service-Level Agreement

## Definitions

**Uptime** The amount of time the service is 
accessible and could return expected response for 
users. Notice that the failures caused by user end
(e.g. network error) are not counted.

**Defect** The unexpected behavior of system 
against the design of service, which is not an 
instant error (i.e. irreproducible bugs).

**Patch**  The installation or injection of 
new code on servers for delivering minor changes (e.g. 
updating user docs) to the service.

**Release** The installation or injection of new 
code on servers for delivering changes, 
new features, or amendments (e.g. adding password 
reset function) to the service.

**Scheduled Maintenance** The preventative maintenance 
that has no effect on user experience and uptime.

**Free User** The legitimate users registered who 
has his/her Email confirmed.

**Pro User** The paid users who have a 
legitimate contract with Crawl.sh.

**API Server** The collection of servers 
that provide utilities including user management, 
job management, payment management.

**Crawl Server** The collection of servers that 
accept and. deal with crawling, which the amount 
of them depends on the amount of active users.

**Frontend Server** The user interface; the collection 
of servers that held static files.



## Service Availability

The uptime is derived by formula:
$$
\text{Uptime} = \frac{h_w - h_d}{h_w} \times 100\%
$$
$h_w$: All hours in a specfic week

$h_d$: Hours in that week the service is not 
accesible returns unexpected responses.

**API Server** shall have 99.9% service uptime 
outside of scheduled maintainence.

**Crawl Server** shall have 80% service uptime for 
free users and 98% service uptime for Pro users. 

**Frontend Server**'s 
service uptime is determined by Google Firebase. 
All frontend contents are deployed on Google Cloud.



## Compensation

When the uptime does not meet SLA, 
a compensation would be given to users. 
The compensation is derived by compensation 
percentage defined in following table:
$$
\text{Compensation} = p \times k_t
$$
$p$: Compensation percentage defined in SLA

$k_t$: The total money user spent in the week the 
SLA is not met

**API Server** 

| Service uptime | Compensation Percentage |
| -------------- | ----------------------- |
| 95% ~ 99.9%    | 50%                     |
| 90% ~ 95%      | 100%                    |
| 85% ~ 90%      | 120%                    |
| 70% ~ 85%      | 140%                    |
| < 70%          | 200%                    |

**Crawl Server** (Pro User)

| Service uptime | Compensation Percentage |
| -------------- | ----------------------- |
| 95% ~ 98%      | 25%                     |
| 90% ~ 95%      | 50%                     |
| 85% ~ 90%      | 100%                    |
| 70% ~ 85%      | 120%                    |
| < 70%          | 200%                    |

**Crawl Server** (Free User)

| Service uptime | Compensation                 |
| -------------- | ---------------------------- |
| 95% ~ 99.9%    | Free Pro account for a day   |
| 90% ~ 95%      | Free Pro account for a week  |
| 85% ~ 90%      | Free Pro account for 3 weeks |
| 70% ~ 85%      | Free Pro account for a year  |



## Measurement

Crawl.sh will monitor and evaluate the servers 
routinely to provide uptime of the service. 

The status of Crawl.sh could be found at 
https://status.crawl.sh

The measurement servers are located in 
different areas to ensure the accuracy of the result.

The measurement servers currently deployed are in:

1. Alibaba Cloud, Shanghai

2. Alibaba Cloud, Hangzhou

3. Alibaba Cloud, Hong Kong

4. Amazon AWS, Tokyo

5. Vultr, Singapore

6. Vultr, London

7. Digital Ocean, San Francisco


## Liability

Crawl.sh is not liable for decrease in Uptime 
due to denial of service (DoS) attacks, 
network floods and hacking not being 
controllable by reasonable measures 
taken by Crawl.sh. In these circumstances, 
Crawl.sh will use commercially reasonable 
endeavours to resolve any issues caused by such an event.
