# 2. AWS Global Infrastructure

## 2.1 Regions
Regions are geographic areas containing multiple Availability Zones (AZs). They are isolated from other regions for fault tolerance and ensure data residency within the region unless explicitly transferred. Selection criteria include:
- Compliance
- Latency
- Pricing
- Service availability
- Feature availability (optional)

## 2.2 Availability Zones (AZs)
AZs are physically separate data centers within a region with redundant power, networking, and connectivity. They are designed to isolate failures within one AZ and are connected to other AZs in the region via redundant fiber.

## 2.3 Data Centers
AWS data centers are secure facilities housing AWS infrastructure with redundant design for power, networking, and connectivity. They are not directly accessible to customers.

## 2.4 Edge Network
- **Edge Locations**: Content caching points for CloudFront (150+ globally) that reduce latency by serving content from the nearest location.
- **Regional Edge Caches**: Larger caches for less frequent content.
- **CloudFront**: A content delivery network service that provides secure content delivery with low latency and supports dynamic, static, and streaming content.

## 2.5 AWS Local Zones
AWS Local Zones are extensions of regions closer to population centers, providing single-digit millisecond latency to local users and enabling latency-sensitive applications to run closer to end-users.

## 2.6 AWS Outposts
AWS Outposts bring AWS services to on-premises facilities with fully managed infrastructure deployed on-premises. They offer the same hardware and software stack as the AWS cloud and provide hybrid capability for a consistent experience.

## 2.7 AWS Wavelength
AWS Wavelength provides computing and storage at the 5G network edge, enabling ultra-low latency applications via telecom providers and eliminating network hops for mobile and edge applications.
