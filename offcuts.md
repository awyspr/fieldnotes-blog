OFFCUTS & NOTES

## 2026-06
~ 5 May https://aws.amazon.com/blogs/awsmarketplace/deploy-aws-marketplace-spg-dashboard-unified-insights/

## 2026-05

## 2026-04
~ 6 Apr
https://awsapichanges.com/archive/changes/080f45-agreement-marketplace.html
2026/03/31 - AWS Marketplace Agreement Service - 8 new api methods

~ 2 Apr
https://awsapichanges.com/archive/changes/080f45-organizations.html
2026/03/31 - AWS Organizations - 8 updated api methods

## 2026-03


NEW-IN-TOWN: Partner Central Agents/MCP compare and contrast Opportunity advice.
Disclosure - using Hubspot as CRM. They're unsuprisingly different and so the value is somewhere in the middle, and most likely operationalized on the CRM side not in ACE. Pull the opportunity summary/recommendations through into CRM, merge/compare with local intelligence that is not synced up, and then decide what to do.

Here's some thoughts/questions that I made note of over the last couple of weeks including as PartnerCentral Agents came into the open. I appreciate these issues/feedback may not all belong to you, but they seem to be in close enough proximity to warrant at least mentioning them.

- On the PCAN call, you mentioned that one future direction would be that partners upload raw/unstructured data to the PartnerCentral Agents - eg call transcripts, documents, diagrams etc. Accepting that some of this might end up in a partner CRM and hence be synced in summary to PartnerCentral anyway, the real question is about what conditions apply to those documents which are typically customer-partner or partner confidential. The hand wavy response is usually that AWS Partner terms apply, but they don't actually address these emerging use cases very well. I am sure a lot of other partners are going to ask this - if we upload this data into PartnerCentral Agents, then does it remain ours ? yours ? shared ? can you guarantee the boundary ie that this won't leak over into another partner (eg competitor).

- Speaking of leakage, I have had a few experiments with asking PartnerCentral Agent about opportunities I have admin access to and specifically about other opportunities for the same customer account that may have been lodged by the primary partner I represent at the time or even _other_ partners. There is certainly some Agent response leakage about what other opportunities may have been registered and the AWS perspective on the customer that comes back. This seems like somewhere some tightening is required. I can give you examples if you like.

- Turning to PartnerCentral Agent advice, I was glad to hear that the Agent has been instructed to "tone it down a bit" in terms of its advice particularly for meeting preparation and sales plan generation - its very long, very prescriptive and most of the time the results are very AWS-seller biased, not partner-business aligned. That seems like a dial you might want to be able to tweak as a partner based on a persona or deal basis or even whole partner-ACE basis - whats the recommendation if I am a partner AE vs an AWS seller, or if I am a supervisor+ of partner AEs vs a territory manager.

- With one partner I work with, we have done some compare/contrast work on pulling (via MCP) the recommendations that the PartnerCentral Agent makes on a deal vs the ones that are made from a CRM-embedded context. This is more typically what a 3PI might do, but there are folks that use CRMs which are connected without a 3PI being involved, and CRMs which have "AI deal advisors". Unsuprisingly - probably because of richer context on the partner CRM side, the advice is often different - sometimes there's an overlap, but the PartnerCentral Agent tends towards "how to do agentic/programmatic co-sell" whereas the partner CRM tends towards "how to close the deal" - you'll appreciate these are not the same all the time. I think the trick will be (and this is probably not new) to combine local intel from a partner's CRM including whatever local agent makes deal progression recommendations with whatever the PartnerCentral Agent gives back on the same deal.


## 2026-02




HOW-TO: Using Resource Explorer vs Cost Explorer for Tagged Workloads

HOW-TO: Mass Tagging for PRM
PRM tagging and exposure of additional info


## 2026-01

MISSING-IN-ACTION: Can't import CloudFormation-based Workload Cost Estimates from calculator.aws into PartnerCentral "Estimator"

HOW-TO: Port Old Estimate to New Estimate

HOW-TO: Create Workload Cost Estimates from CloudFormation
https://docs.aws.amazon.com/cli/latest/reference/cloudformation/estimate-template-cost.html


NEW-IN_TOWN Deal Sizing from Estimates

https://aws.amazon.com/about-aws/whats-new/2025/12/aws-partner-central-opportunity-deal-sizing/


HOW-TO: Service-link ACE Opps with Solution Support
As we reported earlier, you can't attach AWS products/Services to Solutions, nor inherit Products/Services from a Solution onto an Opportunity. So instead, you have to do a two-stepper. Here's one way to achieve the goal without resorting to manual UI click-errors, or needing a 3PI to fill the gap.

Template Products/Services for Solutions

Link Solutions to Opportunities

Iterate Solutions to Link Products/Services to Opportunities using Template

- It would be amazing if you could attach AWS Services to Solutions and then inherit them down to Opportunities which are linked to that Solution. Currently you can't do this, if you want to connect AWS Services to Opportunities you have to do it directly, and at scale the way you do this is to write a query that essentially says "for solution X here is a map of the attached/impacted AWS Services, now go and find all the Opportunities that are connected to that Solution, and then for each of those Opportunities, attach/link the AWS Services that are included in the map". If you use a 3PI, this is logic that they build-maintain, if you don't use a 3PI for CRM you can't do anything with it but flag it for the partner seller that it needs to be added manually (and so it never happens). There will always be the case that for a specific Opportunity there might be non-standard Services attached if its a Solution with a few tweaks around the edges, but currently its a first order problem which is needing to double handle. Whats the ask ? Make it possible to connect AWS Services to a Solution via API, nd then make it possible to inherit that relationship onto the Opportunity.


MISSING IN ACTION - Can't attach AWS Products/Services to Solutions, only from Solutions to Opps (no inheritance) - (Timothy/Tom)

We'll attack this as a two-stepper in a separate post shortly.


MISSING-IN-ACTION: Can't link ProSrv Solutions to AWS Products/Services via API
Another thing thats still not possible is linking Professional Services type Solutions to AWS Products/Services via API.

MISSING-IN-ACTION: Can't edit/maintain Partner Solutions in PartnerCentral via API (Tom/Timothy)
Its a long standing thing, but we're reminded of it while looking at all of the wonderful things you can do with the new PartnerCentral Account API - you can't maintain Solutions. You can link Solutions to Opportunities (or vice versa) as you'd expect and as been available in the legacy  PartnerCentral and in the new PartnerCentral v3.0 (in Console) but you can't create, edit/update Solutions - thats a UI only task.

