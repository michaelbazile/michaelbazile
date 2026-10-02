# Hi, I'm Michael Bazile Jr. 👋🏿

I'm a Senior Software Engineer based in New Orleans. I've worked in education and healthcare, most recently at [TRAILS](https://trailstowellness.org), building software for educators supporting student mental health.

I like having enough context to follow a problem through: from what someone is trying to do in the interface, to the API and data behind it, to what happens when the change reaches production. At TRAILS, that meant working across React, Strapi, PostgreSQL, and AWS, alongside product designers and other engineers.

### A few things I've worked through

- **Imports that outlasted the request.** I moved roster processing into persistent jobs in Strapi's existing database, with cron workers and transactional row locks coordinating claims. The admin UI polled progress and could reopen recent imports. Interrupted jobs stayed available for review because replaying them could repeat onboarding side effects.
- **Search results that needed application context.** I connected Meilisearch and tRPC to Strapi, checking ranked matches against published content and user access, and including prerequisite context for learning modules.
- **Payments that failed after checkout.** I added a path from Lambda to Strapi for asynchronous Stripe failures, recording a terminal billing event without granting access. Existing duplicate-event checks prevented repeated webhooks from rerunning fulfillment.
- **Deployments with a way back.** I built and published four container image variants to ECR and deployed them on ECS/Fargate for the app and website. GitHub Actions handled validation, production approvals, health checks, and recorded rollback targets. Before the website cutover, I tested a release, rollback, and re-release.

### Tools I work with

**Application:** TypeScript, React, Next.js, Node.js, Strapi, PostgreSQL, tRPC, Meilisearch  
**Infrastructure and delivery:** AWS, Docker, Terraform, GitHub Actions  
**Testing and product feedback:** Pa11y, automated tests, Amplitude, PostHog, GA4, user interviews, and code review

### What I'm spending time on

I build personal projects under **Ground & Grow Innovations** and keep working on backend design, infrastructure, and the fundamentals behind them. I enjoy detailed code reviews, working through an issue with someone, and sharing what we learn along the way.

Education and mental health are areas I care about. I want the things I build to have a clear connection to the people using them.

[LinkedIn](https://www.linkedin.com/in/michael-bazile/) · [Email](mailto:mr.michaelbazilejr@gmail.com)
