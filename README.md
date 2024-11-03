# Subnet Calculator - [subnetcalc.com.au](https://subnetcalc.com.au)

Subnet Calculator is a modernized tool based on the original work by [davidc](https://github.com/davidc/subnets).
It strives to be a tool for quickly designing networks and collaborating on that design with others. It focuses on
expediting the work of network administrators, not academic subnetting math.

## Design Tenets

The following tenets are the most important values that drive the design of the tool. New features, pull requests, etc
should align to these tenets, or propose an adjustment to the tenets.

- **Simplicity is king.** Network admins are busy and Visual Subnet Calculator should always be easy for FIRST TIME USERS to
  quickly and intuitively use.
- **Subnetting is design work.** Promote features that enhance visual clarity and easy mental processing of even the most
  complex architectures.
- **Users control the data.** We store nothing, but provide convenient ways for users to save and share their designs.
- **Embrace community contributions.** Consider and respond to all feedback and pull requests in the context of these
  tenets.

## Cloud Subnet Notes

- [AWS reserves 3 additional IPs](https://docs.aws.amazon.com/vpc/latest/userguide/subnet-sizing.html)
- [Azure reserves 3 additional IPs](https://learn.microsoft.com/en-us/azure/virtual-network/virtual-networks-faq#are-there-any-restrictions-on-using-ip-addresses-within-these-subnets)

## Standard mode

- Smallest subnet: /32
- Two reserved addresses per subnet of size <= 30:
  - Network Address (network + 0)
  - Broadcast Address (last network address)

## AWS mode

- Smallest subnet: /28
- Five reserved addresses per subnet:
  - Network Address (network + 0)
  - AWS Reserved - VPC Router
  - AWS Reserved - VPC DNS
  - AWS Reserved - Future Use
  - Broadcast Address (last network address)

## Azure mode

- Smallest subnet: /29
- Five reserved addresses per subnet:
  - Network Address (network + 0)
  - Azure Reserved - Default Gateway
  - Azure Reserved - DNS Mapping
  - Azure Reserved - DNS Mapping
  - Broadcast Address (last network address)

## Credits

Split icon made by [Freepik](https://www.flaticon.com/authors/freepik) from [Flaticon](https://www.flaticon.com/).
Original concept made by [davidc](https://github.com/davidc/subnets)
Modernized version developed by [Caesar Kabalan](https://www.caesarkabalan.com/)

## License

Visual Subnet Calculator is released under the [MIT License](https://opensource.org/licenses/MIT)
