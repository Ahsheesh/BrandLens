# Problem & Scope

## Problem Statement

Build a system that can measure, understand, and improve how a brand appears across search engines, AI assistants,
and AI-generated answers.

### Background

Discovery is shifting from traditional searches or "googling" alone toward AI-assisted discovery, where people increasingly 
ask questions through search engines, chatbots, and answer engines. This changes how brands are found, described, and compared online.

### Problem

Traditional SEO techniques alone are no longer sufficient to understand visibility across AI-driven discovery systems.
Brands need a way to see how they appear in AI-generated responses, compare that visibility with competitors, identify 
gaps in content or positioning, and take action based on those findings.

### Why This Problem Exists

Due to the rise of llms and AI based search engines and the answer systems not surfacing information in
exactly the same way as traditional search engines used to.

### Who Experiences It

Small businesses, freelancers, founders, and independent professionals who want to improve how they are discovered, 
represented, and recommended online.

## 2. Goals

### Primary Goals

- Measure how a brand appears across multiple AI systems, ingest data and construct the brand's current identity.
- Compare brand visibility against competitors and score current standings.
- Identify what users want, product current offerings, and marketing gaps.
- Generate prioritized recommendations to reduce those gaps.
- Track visibility changes over time and measure improvement.

### Secondary Goals

- Support content distribution through social channels.
- Serve small businesses, freelancers, and self-employed users.
- Simulate a realistic professional workflow end to end.
- Keep the system modular enough to extend later.

### Engineering Goals

- Maintain a clean, well-documented system design with no major architectural gaps.
- Make major design decisions explainable with clear alternatives and tradeoffs.
- Include security, maintenance, and test coverage from the start.
- Keep the scope realistic enough to finish within 3 months.
- Present the project at a quality level suitable for internship evaluation.

## 3. Non-Goals

- Not a general-purpose marketing platform.
- The system focuses on AI/search visibility and complements existing SEO workflows rather than replacing them.
- The system does not reverse-engineer or fine-tune LLMs — it treats them as black boxes and observes outputs only.
- Not performing unrestricted web-scale crawling.
- Not being designed for high scale workloads, millions of users and queries.
- Not fully autonomous marketing.

## 4. Users / Actors

### Primary users

Small business owner / freelancer / self-employed professional

### Internal Actors:
- Analysis Engine: collects and processes signals from multiple LLMs and search sources.
- Recommendation Engine: converts gaps into prioritized actions.
- Distribution Module: helps in easy publishing of targeted content to supported social channels.
- Tracking Module: monitors changes over time and stores historical results.
- Admin / Operator: manages configuration, credentials, scheduling, and maintenance.

### External Actors
- LLM providers: return AI-generated answers or summaries.
- Search engines / retrieval sources: provide indexed web visibility data.
- Social platforms: receive distribution content where supported.
- Web sources: pages, articles, and brand references used for comparison and analysis.

## 7. Constraints

- The project must be buildable within roughly 3 months.
- Must be buildable by team of 4 college student, so very limitedly scoped.
- The system is scoped to small businesses, freelancers, and self-employed users.
- External AI and search providers may impose rate limits, quotas, or access restrictions.
- Some social platforms may restrict automated publishing or require approvals.
- LLM responses are probabilistic and may vary across runs.
- All major architecture choices should remain explainable for interview review.

## 8. Assumptions

- Valid brand name with identity that already somewhat exists (not from scratch).
- Publicly observable web content provides enough information to perform useful brand and competitor analysis.
- Observed responses are sufficient to perform black-box analysis.
- Visibility is an observable, probabilistic, useful signals may include brand mentions, frequency of appearance, 
citation presence, competitor presence, query coverage, positioning, and changes over time.
- Visibility improvement can be measured indirectly through repeated observations and tracking.
- Improvements in measured visibility do not necessarily imply improvements in business outcomes.
- Identified gaps can always be converted into actionable recommendations.