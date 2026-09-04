# Platform Team Goals

## Core Mission
- Listen to developers and be empathetic – understand their pain points, workflows, and needs through interviews, surveys, and usage analytics
- Reduce cognitive load on developers – handle infrastructure complexity so developers can focus on their core competency: writing business features
- Treat application development teams as customers and work with them to define best practices

## Developer Productivity & Experience
- Make it effortless for developers to build, test, and ship – remove as much friction as possible from the development lifecycle
- Reduce onboarding time – templatize development environments and workflows so new engineers can start contributing on day one
- Enable "day one" productivity – provide templates for common application types (Go, Java, Python, React) so developers can start committing code immediately
- Improve developer experience – ensure development environments are easy to set up, reduce onboarding time for new developers, and use modern, enjoyable technologies
- Guide teams to write unit tests, integration tests, end-to-end tests, and API tests with platform test infrastructure to make testing easier for developers

## Platform Design & Engineering
- Design, build, and maintain infrastructure and tools that support software development and deployment
- Abstract away infrastructure complexity – hide the complexity of modern cloud-native tooling (Kubernetes, Terraform, Helm, YAML, etc.) so developers can focus on application code
- Provide standardized tools and frameworks to streamline the development process and reduce cognitive load on developers
- Build reusable infrastructure modules (blueprints) – create Terraform modules for common patterns that bake in security, networking, and observability, enabling rapid, consistent onboarding
- Provide building blocks (constructs) with baked-in best practices – create reusable, versioned infrastructure components (e.g., using CDK constructs) that include company-specific policies, encryption standards, security defaults, and compliance requirements
- Publish versioned infrastructure packages – release platform components as versioned packages (e.g., via NuGet, Maven) so teams can consume them like any other dependency, with semantic versioning and release notes
- Standardize the tools and services needed for applications' non-functional requirements (CI/CD, version control, runtime, logging, monitoring, security) across all product teams
- Provide a centralized observability stack – offer shared logging, telemetry, and tracing services so all apps emit data in a consistent way for health monitoring and debugging

## Governance & Best Practices
- Standardize, but enable flexibility – establish opinionated defaults and "golden paths" for core capabilities while allowing necessary room for customization, clearly documenting which areas are negotiable
- Embed best practices and guardrails via Infrastructure as Code (IaC) – create reusable templates with baked-in security, compliance, monitoring, and configuration standards, while still allowing team-specific parameters
- Establish patterns and practices – define consistent approaches for code structure, layer interactions, service communication, and other cross-cutting concerns
- Balance standardization with autonomy – enforce guardrails and consistency where needed, but allow teams the freedom to customize their usage within the platform's boundaries
- Offer flexibility and choice – don't lock teams into a single tool; instead, support multiple standardized options and integrate new tools upon request when they provide value

## Security & Compliance
- Implement security and compliance by default – bake security, governance, and compliance into the platform from the start so teams don't have to think about it
- Maintain security, compliance, and consistency – ensure all platform services meet organizational security policies and regulatory requirements, and provide audit trails and compliance visibility for governance teams

## Reliability & Scalability
- Ensure scalability and flexibility – design infrastructure that can handle increasing workloads and use automation/cloud technologies for seamless scaling
- Guarantee reliability and stability – implement robust monitoring, automated backups, and disaster recovery mechanisms

## Cost Optimization
- Provide cost optimization through the platform – enforce cost-efficient defaults (auto-scaling, resource limits) and track cost savings as a key metric

## Team Composition & Culture
- Have engineers with both development and systems experience – ideal platform engineers have strong programming skills plus operational experience (OS, networking, distributed systems, monitoring)
- Have a stable, dedicated team – the platform team should be a permanent, ongoing team, not a temporary group that disbands after building something
- Blend three skill sets on the team – software engineering (to build abstractions), system skills (to operate reliably), and product/customer empathy (to focus on user needs)
- Avoid being a ticket-taker or bureaucratic bottleneck – don't become a process-heavy team that says "no"; be an enabler that solves problems for developers

## Operations & Maintenance
- Reduce migration pain for application teams – handle upgrades, security patches, and migrations (EKS upgrades, Python version updates) within the platform rather than pushing that work to development teams
- Define and maintain the technology roadmap – guide the organization's technical direction and ensure alignment across teams
- Make strategic technology decisions – answer high-level questions like monolith vs. microservices, cloud provider selection, and other architectural choices
- Evaluate, choose, and integrate third-party tools and services so developers don't have to evaluate them individually

## Collaboration & Support
- Collaborate closely with application teams – understand their pain points, bottlenecks, and workflows, and prioritize platform features that genuinely reduce their cognitive load
- Work with infrastructure/cloud teams – partner with cloud, on-premise, and security teams to leverage their expertise and ensure the platform runs on a solid, well-managed foundation
- Provide clear documentation and support – offer onboarding guides, troubleshooting resources, and responsive support channels to help developers effectively use the platform
- Facilitate collaboration and knowledge sharing across teams – provide technical guidance and promote cross-functional collaboration
- Drive continuous improvement – explore new technologies, tools, and practices to enhance the platform

## Product Mindset
- Continuously develop the platform as a product – treat the internal developer platform like a product with its own roadmap, releases, feature additions, bug fixes, and iterative improvements based on user feedback
- Treat the entire software delivery toolchain as a product – bring isolated DevOps, CI/CD, and operations tooling into a cohesive platform, delivered as a product to internal developers

## Measurement
- Measure migration pain reduction – track how much effort the platform saves teams during upgrades and migrations
