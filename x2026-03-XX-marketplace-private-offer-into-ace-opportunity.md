<a href="https://awyspr.com/"><img src="https://awyspr.com/assets/images/image07.svg?v=b4a015c2" width="10%" height="10%" align="left"></a>

# Turning Marketplace private offers into ACE opportunities

2026-03-XX

## What's this one all about then ?

Text

### Minor heading

Text

```
code block
```

<img src="assets/aws-icons-resource-explorer.png" width="25%" height="25%">

## The wrap up

Text

[Back to awyspr fieldnotes index](https://awyspr.github.io/awyspr-fieldnotes)


2026-03-XX MISSING-IN-ACTION: Turning marketplace private offers into ACE opportunities
It seems pretty reasonable that if you've invested in putting products and services up on AWS Marketplace that you want to be able to kick off an ACE opportunity at the point where a potential customer requests a private offer on Marketplace - right ?

I want to capture an event from AWS marketplace private offer request so that I can create an ACE opportunity from it, using respective APIs and passing the payload between the two. 

This feature is available for the new shiny multi-product solution private offers (see https://docs.aws.amazon.com/marketplace/latest/userguide/multi-product-solutions-faq.html#what-is-ace)

tl;dr you can do this (kick off an ACE opp from a Marketplace action) with "agreement" being the trigger but not "request private offer" being the trigger. 

HOW-TO
Following up from our prior post about marketplace private offers making their way into ACE as opportunities (or more specifically, the fact that you can't do this automagically), we've taken a look at how to use marketplace agreements as the trigger for creating and advancing ACE opportunities. 

The good news - you can do this. 

The bad news - ACE opportunities still need validation, so despite you having an actual agreement for purchase of the product or service from marketplace, syncing that over to the ACE side of the house requires a delay until validation happens, and then advancing the ACE Stage essentially from Approved to Launched in one step.

No matter, lets look at the how.

[steps]

https://docs.aws.amazon.com/marketplace/latest/buyerguide/agreement-eventbridge.html

There's a gap ... no event emitted to trigger this on the marketplace side for a single product opportunity

https://docs.aws.amazon.com/marketplace/latest/userguide/notifications-eventbridge.html#events-for-agreements



There's not a lot of guidance or advice around as to whether or not syncing Marketplace transactions back to ACE opportunities is a desirable thing - but think about it like this - if you have a partner relationship or tier entitlement that is at least partially driven by ACE opportunity lifecycle progression, you're going to miss out on some amount of performance attribution if you have Marketplace business running and are not bringing at least some of those transactions back to the ACE side.
