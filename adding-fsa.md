---

copyright:
  years: 2017,2018
lastupdated: "2019-11-13"

keywords: vlan, add

subcollection: hardware-firewall-dedicated

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}
{:note: .note}
{:important: .important}

# Adding a Hardware Firewall (Dedicated) to a public VLAN
{: #adding-a-hardware-firewall-dedicated-to-a-public-vlan}

A Hardware Firewall (Dedicated) cannot be ordered as part of a server order and must be placed after at least one public compute node is established and the associated VLAN has been added.
{: shortdesc}

To add protection to a VLAN, order a Hardware Firewall (Dedicated) from the VLANs page:

1. From your browser, open the [IBM Cloud catalog ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://cloud.ibm.com){:new_window} and log into your account.
2. Select the Menu icon ![Menu icon](../../icons/icon_hamburger.svg) from the top left, then click **Classic Infrastructure**.
3. Select **Network > IP Management > VLANs** to go to the VLANs page. Each row represents a VLAN in your infrastructure. IBM© Cloud populates the "VLAN Number" and "Primary Router" information automatically, indicating the true VLAN number and the router that it is configured on. The "Name" field can be used to define a recognizable name. The far right column "Gateway/Firewall" contains details about what firewall protection, if any, is in place for that VLAN.

	To filter the VLANs table to only show public VLANs, click on the **Filter** tab, enter "fcr" in the Primary Router field and click the **Filter** button.
  {: tip}

4. Find the VLAN you want protected and click the **Add Firewall** link in the same row. This link opens the **Order Hardware Firewall (Dedicated)** page. If the "Gateway/Firewall" column is already populated, a Firewall or Network Gateway is already associated with the VLAN and the device must be removed before you can proceed.
5. Select **Hardware Firewall (Dedicated)** or **Hardware Firewall (High Availability)**.

	The High Availability option deploys the same hardware and interface, but deploys a second passive node to continue processing traffic if the active node fails. High Availability reduces the risk of excessive downtime.

6. Click on the **Servers on this VLAN** button to verify you are selecting the appropriate VLAN.
7. Enter your choice of payment and click **Continue**.
8. In the next screen, enter promo codes if applicable, read and agree to the Master Service Agreement and click on **Place Order**.
