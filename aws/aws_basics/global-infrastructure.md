# AWS Global Infrastructure

AWS provides infrastructure in all continents, except Antartica.

## Region

Physical location around the world where data centers are clustered together.

A group of logical data centers is called an Availability Zone.

Each AWS Region consists of multiple, isolated and physically separate Availability Zones within a geographic area.

## Availability Zone (AZ)

Zoned area within a Region that can harbor one or more data centers, tipically 3.

It houses all the hardware devices that AWS offers.

With their own power infrastructure, the AZs are phisically separated by a meaningful distance (up to 100KM) from any other Availability Zone in the Region.

AZs are interconnected with high-bandwidth, low latency networking, to provide low-latency networking between zones that is sufficient to accomplish synchronous replication.

## Edge Location

Edge locations are connected to the AWS Regions through the AWS network across the globe. They link with tens of thousand of networks for improved origin fetches and dynamic content acceleration.

Edge locations cache copies of your content for faster delivery to users at any location. They support AWS services like Amazon Route 53 and Amazon CloudFront.

AWS has over 200 edge locations that are placed in 90 cities, across 47 countries.
