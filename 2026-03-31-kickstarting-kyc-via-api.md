<a href="https://awyspr.com/"><img src="https://awyspr.com/assets/images/image07.svg?v=b4a015c2" width="10%" height="10%" align="left"></a>

# Kickstarting KYC via API

2026-03-31

## What's this one all about then ?

Overnight AWS released a couple of small but significant API methods on the PartnerCentral Account API.

### The changes

There are two new methods on the PartnerCentral Account AI regarding verification.

* ```StartVerification``` - Initiates a new verification process for a partner account. This operation begins the verification workflow 
for either business registration or individual registrant identity verification as required by AWS Partner Central. 
[Details here](https://docs.aws.amazon.com/partner-central/latest/APIReference/API_account_StartVerification.html)

* ```GetVerification``` - Retrieves the current status and details of a verification process for a partner account. This operation 
allows partners to check the progress and results of business or registrant verification processes.
Again [details here](https://docs.aws.amazon.com/partner-central/latest/APIReference/API_account_GetVerification.html)

So why do these matter ?

In AWS world, KYC is not a one and done process.

For a lot of AWS partners, KYC (at least in the form of verification) came back with the PartnerCentral v3.0 migration.

But periodically it comes up too - every couple of years, AWS forces a partner to reverify.

If you're changing your legal name or involved in an M&A process (merging, acquiring, creating trading subsidiaries), it 
will happen as well. And if any of that crosses geographic/jurisdictional boundaries, its another trigger.

If you change your Partner Alliance Lead, verification of their role is also required.

And thats before a similar process for Marketplace (although KYC there is much stricter for sellers as its related to
disbursements of funds - real money flowing that has compliance requirements).

If you are a 3rd party integrator - eg supporting CRM integration with ACE or publishing to Marketplace, you'll often encounter
a verification wall as well, and historically that's meant a loop out to the Partner Alliance Lead to get something fixed/

So with these two new methods, verification and light KYC processes can be kickstarted over an API rather than using an
older style workflowed form.

## The wrap up

Being able to kickstart verification without the older style form process is very helpful. Its another step
on the partner integration-automation journey across an infrequent but important process for AWS partners.


[Back to awyspr fieldnotes index](https://fieldnotes.awyspr.com)
