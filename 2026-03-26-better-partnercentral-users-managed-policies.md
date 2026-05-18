<a href="https://awyspr.com/"><img src="https://awyspr.com/assets/images/image07.svg?v=b4a015c2" width="10%" height="10%" align="left"></a>

# Better PartnerCentral Users and Managed Policies

2026-03-26

## What's this one all about then ?

This week AWS shipped a significant (but not well-advertised) update to PartnerCentral Users and IAM Managed Policies.
For AWS partners who did not cross the PartnerCentral 3.0 in Console migration bridge yet (clock is ticking ...), or even for those who went early
and battled the lack of detailed documentation (bravery awards are coming), this is a really useful thing.

### Before ...

Early on migrations for PartnerCentral were "interesting" because of the lack of translation for the different types of roles and permissions
in the legacy PartnerCentral portal and the disconnect against the new world of IAM managed policies which seemed fairly coarse grained. 

Quite a number of partners we worked with and forums we participate in featured advice like "make lists of your groups, existing memberships and 
existing permissions and then replicate them temporarily in IAM to make sure that everyone that used to have access to something has it in the new 
world". It was doable, but ugly at scale.

### After ...

There's two parts of this.

One is the new set of [AWS PartnerCEntral User Personas](https://docs.aws.amazon.com/partner-central/latest/getting-started/managed-policy-mappings.html#common-personas). This table - unhelpfully compressed and scrolling in the doco - is the new bridge between worlds, and essentially 
replaces the manual mapping of the legacy state. It lists an AWS PartnerCentral User Persona (in terms that a Partner Alliance Lead will understand) and connects it to a specific IAM Managed Policy (in terms that a systems administrator will understand).

The other is its pair, in [IAM change history](https://docs.aws.amazon.com/partner-central/latest/getting-started/managed-policies.html#security-iam-awsmanpol-updates). This table lists every PartnerCentral managed permission set, and what it can and can't do (ie things people can see or not if they are given the role).

## The wrap up

Moving from the legacy version of PartnerCentral and into the new v3/Console experience is a very important activity for 
Partners in 1H/26. Many many new features of the AWS partner journey and AWS support for progression and engagement assume
that you've migrated. These new mappings and managed policies help ease some of the change burden.

[Back to awyspr fieldnotes index](https://fieldnotes.awyspr.com)
