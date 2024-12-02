# IOC Decay Automated by Tines
The question of IOC decay came up when we decided to automate the blocking of IOCs on the border firewall.  

How long should IPs stay shunned?

When do Indicators of Compromise begin to age out and become irrevalent?

7, 14, 30 days?  

Phishing campaigns can cycle through IPs very quickly, so is there merit to blocking IPs for a long time?

What about domains used in phishing or malware campaigns?

This question came up when I started work on blocking domains in Cisco Umbrella with Tines.

After some research, I came across a blog on the Dragos website, which provided a good framework for assessing IOC decay and confidence.

How long should IOCs be blocked? 

It depends according to the authors of the Dragos article. You need context in regards to maintaining IOCs on block lists. According to the authors, the following keys are used for success: 

- Build a set of trusted IOC sources.
- Use automation for when leveraging IOCs in SecOps. 
- Deriving value from IOCs by timely deployment.

With Tines, I can use their automation platform to leverage and to lifecycle IOCs in all our security solutions.

Check out my [previous blog](https://automatesecops.github.io/Working-With-Tines-Resources/) where I use Tines Resources to manage and lifecycle IOCs.

Tines can ingest IOCs and provide protection across our entire security infrastructure, in a timely manner.

I hope you found this useful.

Once you start automating, you can't stop.

Happy Building.

Tom

P.S.
Before I started the automation of blocking IOCs, I took an inventory of the IOCs already in place. In the GitHub repo, I uploaded my Tines Story for collecting blocked domains in Umbrella.



- [Dragos Blog on IOC Decay](https://www.dragos.com/blog/end-of-life-of-an-indicator-of-compromise-ioc/)

## Tines Documenation
- [Tines Resources](https://www.tines.com/docs/resources/)
- [Tines Object Function](https://www.tines.com/docs/formulas/functions/object/)
- [Tines Append Function](https://www.tines.com/docs/formulas/functions/append/)
- [Tines Append Element to Resource](https://www.tines.com/api/resources/append-element/)
- [Tines Pagination Examples](https://www.tines.com/library/stories/91375/?name=implement-pagination-with-these-techniques)
- [Tines Community Edition](https://www.tines.com/pricing/)

[Previous Blog](https://automatesecops.github.io/Working-With-Tines-Resources/)
