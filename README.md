# axe-fast
axe-fast is a project to make [axe-core]() faster and more efficient. EqualifyEverthing publishes this repo as a public placeholder for future awesomeness we’ll release under an open source license. 

## Why release a repo with no code?

Open sourcing code only makes sense if folks are interested in contributing to it, and this repo helps gauge interest in axe-fast. 

Show your interest by starring the repo and adding feature requests or questions as issues. Once a critical mass of folks express interest, we will open source code that’s currently private. 

**Side Note:** Equalify does sponsor development. If you’re interested in contributing but need cash, checkout #1. 

## Why is Equalify working on this?

We aim to “equalify” 100,000,000 accessibility issues by 2028.

A faster and more efficient axe means more pages can be scanned. More scanned pages, coupled with [Equalify’s platform](), means more accessibility issues are marked “equalified.” An equalified issue is a fixed issue. Let’s fix accessibility problems at scale!

## Key Questions
Our development is focused on answering these key questions:
- **How can we speed up large tests?** Tests like checking all page elements for color contrast errors is too slow. We’re exploring ways, such as reduced reliance on Selenium, to speed up big tests.  
- **How can we leverage languages that are built to optimize performance?** Particularly, we’re looking at how [Rust]() can deliver deliver high performance safely.
- **How can we responsibly deliver to the Equalify platform lots of alerts that are scanned from lots of pages?** Equalify makes accessibility data useful when scanning really large site networks (10k+ pages). With an average of 50 alerts per page, we’re building a solution that can deliver at least 50k alerts to Equalify. 

## Requirements
In developing our solution, we need to fulfill certain requirements so that we can support future development:
- The solution must be accessed and controlled via a REST API, so that Equalify and other services can easily interface with it.
- The solution must accept and process  up to 10,000 pages at once by ingesting URLs. These URLs are currently delivered via an XML site map, but that can change. 
- The solution must be deployable as a web service. We plan to sustain future development by charging users a nominal amount to use the SaaS.
- Last but certainly not least, the solution must be significantly more efficient than axe is currently. Our existing work aims to test 1200 pages in the time it takes axe to test 1 page. 

## Any questions?
Please post an issue! We’re curious to see how this develops. 
