

Cloud Computing



* The delivery of computing services:over the internet with the ability to be flexible (scaleable), perform computing tasks faster and benefit from economies of scale
    * Storage
    * Servers
    * Networking
    * Databases
    * Software
    * Analytics 
    * Artificial intelligence
* Benefits of the cloud
    * Available on demand; no need to setup infrastructure
    * Cost effective
        * Only consume what is needed
        * Able to expand requirements quickly and cheaply (not paying for unused resources)
    * Accessible anywhere with internet connection

Shared Responsibility Model



* The shared responsibility model outlines the responsibilities of the customer and the cloud vendor
* The cloud vendor is responsible for the security of the cloud but the user is responsible for security in the cloud such as their applications or user account details or whom can access their data stored on cloud infrastructure
* Cloud vendor is responsible for managing physical access to computing resources
   * Hosts
   * Network
   * Datacentres
* The customer is responsible for:
    * Information and data
    * Configuration 
    * Users and group accounts and identities
* Depending on the cloud model being implemented, the following may or may not be customer responsibilities:
    * Operating system					Infrastructure as a service
    * Networking / Application environment / Identity	Platform as a service
    * Applications						Software as a service

Public Cloud



* Owned and operated by a third-party
* Microsoft Azure, Google Cloud Platform, DigitalOcean and Amazon Web Services are examples
* These services require an internet connection
* These offerings are usually cost-effective, scalable and flexible
    * No upfront costs
    * Easy to access
* Shared tenancy which may not be appropriate for privacy-focussed applications (whether its mandated by law or best practice)
* Lots of different applications
* Eliminates the need for organisations to maintain their own hardware

Private Cloud



* Cloud computing resources provided for a single organisation and maintained over the intranet (private network)
* Usually the hardware is provided onsite but may be maintained by a third-party (but only accessible for a particular organisation)
* Usually used my governments
* Provides greater security and privacy for data-sensitive material
* More expensive and not necessarily scalable the way the public cloud is 

Hybrid Cloud



* A mix of private and public
* Data can mix between private and public cloud entities
* Data-sensitive stuff stays in the private cloud but organisation gets the benefits of the public cloud 
* Connections are private using a VPN or Azure ExpressRoute
* Requires more managing and responsibility by the customer but offers more flexibility in allowing some servers to be run locally instead of off the cloud

Multi Cloud



* A subset of hybrid cloud where multiple cloud providers are used and even connected to each other
* This can have many benefits such as:
    * Risk diversification
    * Avoid vendor lock-in
    * Optimise workloads by using the best cloud vendor for a specific resource
* There are also negatives too:
    * Increased complexity 
    * Interoperability challenges since each cloud provider may do things their way and perhaps different to a different cloud provider
    * Resource fragmentation (you may be using two different cloud providers that both offer virtual computing but now you have two opportunities to waste unused resources)
    * Requirement for data transfer between clouds which may have extra costs (time or money) and extra vulnerabilities (more points of failure)

Azure Arc



* Enables the user to utilise Azure management (such as Azure monitoring tools or Azure management tools via powershell) on non-Azure resources
    * Servers (Windows or Linux / Virtual or bare-metal)
    * Kubernetes 
    * Databases / SQL servers
* We can use Azure services for third-party resources such as:
    * Policy
    * RBAC
    * Tagging
    * Defender
* The main use case for Azure Arc is to unify different systems under one roof
    * One example is monitoring a computer that is acting as a server that is not virtual and not directly connected to Azure; we can use Azure Arc to enable us to monitor and interact with this computer as if it was on the cloud

Economy of Cloud Computing



* Capital expenditure (CapEx) - Cloudless infrastructure
    * Large upfront investment
    * Very high initial capital expenditure
    * Often have to overprovision 
    * Includes costs such as infrastructure, land, building, setup costs
    * You own the equipment and the risk
    * Tax deduction may be available
* Operation expenditure (OpEx) - Cloud infrastructure 
    * No initial upfront cost
    * Pay as you go
    * Pay for only what you need right now
    * No need to forecast for long-term needs

Infrastructure as a Service (IaaS)



* Networking, **virtual machines** and storage are provided by the cloud provider
* Pricing is based on what resources you have been allocated (CPU / RAM / storage) and usually users are given tiers to choose within
* Provides the most fundamental components of cloud computing
* The user has to manage the application, data, runtime, user management, networking, middleware (such as an nginx server or Apache Kafka or a game engine) and operating system
* This service type gives the customer the most flexibility and the most responsibility
* Examples include Amazon Web Services (AWS) EC2, Microsoft Azure Virtual Machines, and Google Compute Engine

Virtual machines



* Virtual machines consist of:
    * CPU
    * RAM (memory)
    * Storage (disk capacity)
    * Networking
    * Networking controls (firewall)
    * Operating system
* Virtual machines run on physical servers (hypervisors) running Microsoft Hyper-V or VMware
* Multiple virtual machines may be run on a single physical server
* Virtual machines have the same capabilities as a physical computer
* Virtual machines have many advantages over physical machines
    * Scalability (can use as much or as little resource as you are willing to pay)
    * Instant (can wind up a virtual machine instantly)
    * Redundancy (if virtual hypervisor host machine fails then its very easy to spin another one up on a different server)

Platform as a Service (PaaS)



* Applications such as the operating system, development tools, middleware, database management are included on top of the infrastructure 
* Anything that is an application but requires a user to 'configure' is considered as PaaS
* PaaS is considered a 'fully managed' service
    * Users don't need to worry about computing power / hardware
    * Cloud vendor is responsible for operating system updates, software licences, server maintenance, database management and auto-scaling
* Some common uses of PaaS include:
    * Software development / DevOps pipelines
    * Web app development
    * Storage services 
    * Managed database
    * Security solutions such as firewalls
    * [Business] Analytics
* Disadvantages to platform as a service vs. infrastructure as a service
    * Less control on infrastructure
    * Limited choice of tools provided by the cloud vendor
    * Application compatibility such as being forced to use a particular programming language
* Examples include Heroku, Google App Engine, and Microsoft Azure App Service

Function as a Service (FaaS)



* A subset of platform as a service
* The user is responsible for the application (programming)
* Basically this service is 'serverless' and all the cloud provider does is run the function
* Usually the code is a small self-contained function in whatever programming language that may be triggered based on an event (such as database changes or file upload or scheduled cron job)
* Examples include AWS Lamda or Microsoft Azure/Google Cloud Functions
* Common example use cases of FaaS include:
    * Microservices
    * Batch processing
    * Internet of Things
    * API creation

Software as a Service (SaaS)



* Software applications running off the web
* Cloud providers provide pretty much everything including the software
    * Customer does not need to worry about developing the application
    * Customer does not need to worry about allocated resources or orchestration tools or monitoring software or networking
    * Customer does not need to worry about licensing 
    * Customer does not even need to be tech savvy
* Customers are responsible for
    * Accounts and identities
    * Device security
    * Data access permissions
* This service type gives the customer the least flexibility and the least responsibility
* Pricing is based off a subscription based model (pay per week/month/year)
* General public will generally associate cloud with software as a service
    * Email
    * Customer relationship management (CRM) such as Salesforce
    * Enterprise resource planning (ERP) systems
        * ERP is a software package which integrates multiple functions such as finance, accounting, human resources, supply chain management, manufacturing, sales, and customer relationship management
        * Microsoft Dynamics 365 is a CRM and ERP toolkit
    * Collaboration tools 
        * Microsoft Teams 
        * Zoom
        * Slack (AWS based)
    * Productivity tools
        * Microsoft Office 365
        * Google Docs

Benefits of Cloud Computing



* High availability
    * Availability is how accessible a computing resource is; if I want it can I get it
    * High availability is provided by redundancy 
        * Multiple data centres mean if one data centre crashes then another can take over
        * Multiple connection points mean if one geographical area loses networking then another connection point can be utilised
        * Virtual machines can spin up instantly so when one breaks another can take over with minimal down time
        * Load balancing which is often automatically provided by cloud vendors can ensure one server does not become unresponsive with excess demand for its resources 
    * Availability is important for businesses that have critical components that require to be running all the time such as:
        * Websites
        * Communications
        * Data access such as media streaming or software distribution
* Scalability
    * Scalability is the ability to increase workload by adding more resources (horizontally or vertically) and the cloud is perfect for this since its resources are almost limitless and it is very easy to add resources 
    * Easily distribute traffic or resources amongst several servers via a load balancer (note load balancing is not exclusive to cloud computing)
    * Shift the load to different geographical regions to reduce latency for particular regions (utilise a server in Hong Kong for applications in Cantonese)
    * Horizontal scaling (scaling out) is how cloud computing achieves most of its scaling by:
        * Adding more virtual machines to handle the computing load using infrastructure as code
        * Utilising a load balancer to distribute the load evenly amongst multiple servers (virtual machines)
    * Vertical scaling (scaling up) involves increasing the computing power of an existing server or virtual machine and is not often utilised when using cloud architecture
        * This usually involves adding CPU or RAM or disk space
        * This type of scaling is usually manual and involves downtime (server must be temporarily turned off to upgrade)
* Elasticity
    * Elasticity is the ability to increase (or decrease) resources to meet demand 
    * It is a 'special type' of scalability
    * An example of elasticity in the cloud is **cloud bursting**
        * Cloud bursting is where a private cloud utilises the public cloud when resources on the private cloud are stretched
        * This allows the private cloud to maintain critical applications whilst utilising the resources of the public cloud to maintain uptime
        * Users only pay for public cloud during cloud bursting episodes
        * An example use case for cloud bursting would be tax companies performing activities before tax deadlines
* Reliability
    * Reliability is the ability to recover from disasters or failures; if I have it will it work consistently
    * Cloud technology achieves this:
        * No single point of failure (multiple failures must occur before a computing resource is offline) by having a decentralised design 
        * Redundancy by offering a resource from multiple locations in the world (global scale) which can protect against regional / geographical disruptions
* Predictability (Performance)
    * Predictability is the consistency of performance of an application (or virtual machine) running on the cloud
    * Cloud technology achieves this by:
        * Auto-scaling
        * Having high availability
        * Load balancing
    * Regular technology can also achieve this by
        * Providing excess resource
        * Utilisation of standard practices and containerisation 
* Predictability (Cost)
    * Estimating costs can be achieved by various tools that cloud vendors provide to their customers
    * Tools can also optimise how users use the cloud to find the most efficient package for their needs
* Security
    * Security control is somewhat based on the service type
        * IaaS gives users full control of operating system security
        * This also means users have more responsibility
    * Network security is largely handled by the cloud vendor whom will provide
        * DDoS protection
        * Network load distribution
        * Advanced monitoring tools
        * Network filtering 
            * Firewalls
            * IP blacklist / whitelist
            * Rate limiting protocols
* Governance
    * Governance is a collection of policies, processes and controls that dictate the minimum standards for using cloud computing resources 
    * Cloud vendors implement many of these standards including
        * Enforcing encryption standards
        * Data location and storage restrictions 
        * Providing auditing tools to comply with regulations
        * Providing automatic updates and patching 
    * Cloud vendors help users meet regulatory requirements such as
        * GDPR (General Data Protection Regulation - EU privacy law)
        * HIPAA (Health Insurance Portability and Accountability Act - US healthcare information privacy laws)
        * FISMA (Federal Information Security Management Act - US government operations and information privacy rules)
* Manageability
    * Manageability of the cloud using automation tools
        * Auto-scaling to increase resources to meet demand
        * Monitoring with automated alerts or custom actions triggered by events
        * Template-based deployment to automate workflows such as deployment
    * Manageability within the cloud
        * Web portal (GUI)
        * Command line
        * APIs

Azure Regions



* A region in Azure is as:
    * Set of data centres
    * Near each other (from a latency point-of-view)
    * Connected data centres utilise a dedicated high-speed network 
* Each data centre within a region has its own power, utilities and network infrastructure 
* Most regions are located in important geographical locations (such as city hubs)
* Regions are connected together by Microsoft's own optic fibre network that sprawls along the oceans (not on the 'internet')
* When we deploy Azure resources we need to select a region to host it
    * Location closest to our users (minimising latency) is usually the default option
    * Some features are only available at certain regions
    * Price varies between different regions and may be a factor in the selection process
* Regions have a 'pair' which is another collection of data centres that are geographically close 
    * These region pairs facilitate redundancy (so if one region has an outage the region pair can take over)
    * Maintenance can occur in one region and the region pair can continue operation
* Sovereign regions are special regions that are isolated from the global cloud
    * They are not part of the Azure public cloud
    * Sovereign regions are primarily used by the US governments (security reasons) or the China region (comply with Chinese law)
        * Approval must be granted before resources can be deployed onto special regions 
            * In the US, only government contractors or government departments have access 
            * In China, only businesses in China can utilise the Azure China region (and they can only access China region)
    * Some services are not available

Availability Zones



* Inside a region are separate availability zones
* Each availability zone has independent:
    * Power
    * Physical security
    * Connected to each other with high redundancy (duplicate connections)
* Each availability zone will be comprised of at least one data centre
* Each region will have several availability zones 
    * Generally a minimum of 3 zones per availability zone
    * Each zone has a 2ms or less latency between each other (so they usually quite close to each other)
* Availability zones provide redundancy which improves availability (and reliability)
    * Zone redundancy is where a service or resource such as storage is replicated amongst different data centres within an availability zone 
    * When we deploy a resource in Azure, we are given the option to:
        * Select which zone within a region 
        * Select zone-redundancy (available for services like storage) 
    * Zone redundancy is provides higher availability but it comes at a cost

Azure economy



* A set of guidelines for building tools on the Azure platform
* Cost optimization
    * Plan for estimated costs using various monitoring tools
    * Utilise tools to optimise resource allocation based on cost
* Operational excellence
    * Implementing DevOps 
* Performance efficiency
    * Automating scaling to meet computing demands
    * Identify and minimise bottlenecks in developing applications
* Reliability
    * Maintaining uptime
        * Achieving high availability
        * Eliminating single points of failure
    * Recover from data loss
* Security
    * Implementing defence in depth

Identity



* Identity in Microsoft Azure is who a person claims to be or what an object claims to be
* Examples of physical identities include:
    * Driver's licence
    * Passport
* Examples in the digital world include:
    * Software licence
    * Azure Active Directory objects
    * Email address
    * Certificate (for applications)
* In Azure, we use the term **security principals **to define identities that can be assigned a role such as
    * Users
    * Groups
    * Service principals
        * Service principals are 'users' that are applications which access other Azure resources
        * An example would be a powershell script that stops a virtual machine (it needs authorisation to stop a virtual machine)
        * Third party applications like Microsoft Teams can also access Azure resources (if permitted) and they will have a service principal made for them in the the Azure Active Directory (tenant)
        * Service principals are identities stored in Azure active directory and acts as a middleman for authentication between two different Azure resources
            * Application 1 sends a request to the active directory
            * Active directory sends an authentication token back to application 1
            * Application 1 then sends this authentication to application 2. In this step, the token needs to be temporarily stored somewhere in the application code
            * Application 2 sends this authentication token to the active directory
            * Active directory validates the token and sends the request back to application 2
            * Application 2 then allows application 1 to access its resource
    * Managed identities
        * Managed identities are a special type of service principals that bypasses the need to store credentials on applications, thus reducing the danger of storing secrets within applications
        * Managed identities facilitate communication between applications and Azure resources and come in two flavours:
            * System assigned 
                * When the Azure resource is deleted, so is the managed identity
                * It allows one application to access one Azure resource
            * User assigned
                * Allows one managed identity to connect to many Azure resources (and an Azure resource can connect to many user assigned managed identities)
                * Removal of an Azure resource does not delete a user assigned managed identity

Authentication



* Authentication is the process of verifying an identity
* Examples of authentication in the physical world include:
    * Keys to a building
    * Certificate of authenticity
    * Keycodes for a lock
* Examples of authentication in the digital world include:
    * SSH keys
    * Passwords
    * SSL certificates

Authorisation



* Authorisation is the process of validating what an identity can do at a particular place at a particular time
    * Examples of authorisation in the physical world include
        * A ticket to an event
        * Key card
    * Examples of authorisation in the digital world include:
        * Application secrets
        * Shared access signature (SAS) tokens

Access Management



* Access management is the control, verification and tracking of authorised users and applications
* Access management in Microsoft Azure is provided by Azure Active DIrectory (also known as Entra ID)

Azure Active Directory / Entra ID



* Microsoft Entra ID is a product family that includes:
    * Azure Active Directory
    * Permissions management
    * Verified ID
* Azure Active Directory is the cloud-based active directory
    * The improvements Azure Active Directory makes over Windows Active Directory
        * Cloud-based (accessible anywhere) instead of relying on an on-premise server running Windows Active Directory
        * Built on the modern web so it integrates with modern web applications whereas Windows Active Directory is built on legacy services and does not integrate well with modern web applications
        * Utilises modern authentication protocols such as multi-factor authentication
* Azure Active Directory Domain Services (AADDS) enables the use of legacy Windows Active Directory on cloud technology
    * This removes the need for organisation to run a Windows Active Directory server on-premise and maintain said server
    * It integrates well with Azure Active Directory
    * This is an example of a hybrid-cloud interaction
* Characteristics of Azure Active Directory
    * Comes standard with any Microsoft Azure account
    * Requires at least one user to run 
    * Only the global administrator has full power to assign roles, add/delete/modify users/groups and grant users/groups permissions
    * Can be paired with a custom domain or connect to an existing on-premise active directory server using Azure Active Directory Connect or use a domain provided by Microsoft
        * Azure Active Directory Connect allows for users and groups on an active directory (on-premisr) server to be synchronised and a copy of their identities can be stored in Entra ID / Azure Active Directory 
        * This allows existing users from an on-premise Active Directory can be granted access to Azure resources without creating a new account 
    * Each organisation has its own instance of Azure active directory (known as a tenant) which has its own domain (Microsoft based or custom)
        * Users can be members or guests of multiple tenants and have a max limit of 500 different tenants
        * Members of tenants are given access to various resources within Azure such as Virtual Machines or Blob Storage
        * Tenants can have multiple billing entities (subscriptions) which can separate costs amongst different groups of users

Azure Active Directory Domain Services (AADDS)



* Azure Active Directory Domain Services is useful for organisations that use or require the use of legacy applications or legacy active directory protocols
* Some examples of legacy active directory protocols include:
    * LDAP (Lightweight Directory Access Protocol)
    * NTLM (New Technology LAN Manager)
    * Kerberos
* AADDS offers Windows Active Directory server on Azure infrastructure
    * Removes the need for managing an on-premise active directory server
    * In built fault tolerance and redundancy (a minimum of two virtual machines are active when using AADDS)
    * A domain (or a custom one) is given for easy access
    * Offers integration to Microsoft Azure Active Directory (Entra ID)
        * User and group information from Entra ID can be copied onto an AADDS instance
        * Note Entra ID can connect to an on-premise active directory and either copy its users/group information to the on-premise server or copy the on-premise server user/group information allowing users to use their active directory (non-cloud) login to access Azure services

Microsoft Entra ID (Azure Active Directory) Identity Protection



* Identity Protection is a service that uses analytics and machine learning algorithms to detect suspicious logins and can elevate required credentials for suspicious logins
    * It can implement risk-based conditional access policies
    * An example would be if a user logs in with an IP address from an atypical country, then multi-factor authentication may be enforced
* Some features of Identity protection include:
    * Blocking access to an account 
    * Mandate resetting passwords 
    * Enforce multi-factor authentication
    * Reporting of suspicious login attempts
    * Password vulnerability assessments
* Conditional access relies on signals and decisions
    * Signals can include:
        * IP address of client
        * Device health
        * Device compliance
        * Application used to connect
        * Real-time risk detection
        * User or group logging in
    * Access decisions are the actions that take place when a risky login is detected
        * Granting access
        * Enforcing MFA
        * Limiting access with session controls
        * Blocking access
    * Conditional access requires a premium Entra ID subscription 

Zero Trust Model



* The zero trust model is a security concept that establishes the 'do not trust anyone' belief and that in order for trust to be established, verification / authentication must occur for all users
* The idea of zero trust model is that threats can be external and internal
    * This model of defence differs slightly to the 'defence in depth' model where security is based on the concept of having multiple layers
    * The **trusted perimeter model **attributes trust to users within the same network but this creates issues such as:
        * Internal threats are unprotected
        * External users have difficulty accessing the secured network which makes it difficult to facilitate remote access or grant access to third-parties without using a VPN (virtual private network)
* Zero trust model involves implementation of several key concepts
    * Implementing access control policies
        * Users only get access to what they need (least privilege of access)
        * Assess user's device health and location (IP address)
        * Governance of access is handled by a centralised entity (such as Microsoft Entra ID)
    * Segmenting access into separate zones
        * Users are granted access to zones
        * Access to one zone does not allow access to another unless the user has access to both zones
        * Often organisations will have a zone that has external access (suh as a website) but keep the back-end in a separate zone that is inaccessible from the outside 
        * This limits the damage done from an internal threat to the affected zone(s)
    * Multi-factor authentication
        * Multi-factor authentication is the principle of using multiple methods to verify the identity of a user
            * Something the user knows (password)
            * Something the user has (a mobile device)
            * Something the user is (a fingerprint or face unlock or retina scanning)
        * This solves the issue of threats only needing to know one piece of information to gain unauthorised access
        * Multi-factor authentication does have some issues:
            * Often reliant on secondary device; if secondary device is not available then a backup method is required or access will be unobtainable
            * It is more frustrating for users 
    * Passwordless authentication 	
        * An alternative to password which are inherently insecure
        * Passwordless authentication includes:
            * Physical devices (keyfob or phone)
            * A part of the user (fingerprint or face)
        * Microsoft Azure accepts multiple passwordless solutions:
            * Microsoft Authenticator App 
            * Windows Hello
            * FIDO2 security (hardware) key
                * NFC tag
                * Bluetooth
                * USB device
                * Biometric 
    * Conditional access
        * Adds an extra layer of protection that grants users access based on certain conditions; conditions that generally unauthorised third-parties cannot meet such as:
            * Location (IP address)
            * Device-specific 
                * Platform OS
                * Devices that belong to the organisation
            * User/groups (user must be part of a particular group)
            * Application (access is granted if user is using a particular application such as database access granted to a website server)
            * Multi-factor authentication 
        * Conditional access can also be changed to block access
            * Block access using legacy authentication protocols
            * Block access if multiple sign-in failures occur

Azure Microsoft Authenticator



* Facilitates the use of one-time passwords with the Microsoft Authenticator Application
* This service can offer:
    * Biometric authentication
    * Send push notifications to users to prompt login attempts
    * Multi-factor authentication
    * Enable the use of OATH tokens with Entra ID and third party identity providers

External Guest Access



* Implementing security policies creates new challenges in allowing third (external) parties access to an organisation's network / resources
* There are multiple ways we can handle this problem
    * Make the external user an internal user account
        * External user now has to juggle a new account
        * Requires the need for identify internal and external users in IAM software
        * Increases the number of identities that an organisation needs to manage
    * Permit the external user to have access using their existing account
        * Requires trust between the internal and external parties
        * Requires the external account to have features that are compatible with the internal organisation's security policies
* Microsoft Azure offers two different services for external guest access
    * Entra External ID for partners (Azure Active Directory B2B)
        * Grants access to third parties to access an organisation internal network 
        * External users are given an identity inside the organisation's active directory
    * Entra External ID for customers (Azure Active Directory B2C)
        * Grants access to 'users' (customers) to external facing resources such as applications or websites
        * Users can use an existing account (such as a Google or Facebook account) to access these resources
        * The third party shares some information with Azure Active Directory B2C and a new user object is created 
        * These users cannot access the organisation's internal network, only what is publicly accessible 	

Role Based Access Control (RBAC)



* RBAC is the system for governing access based on 'roles' which are given to users
* Azure active directory (Entra ID) uses RBAC model to grant permissions to users/groups
    * Users in a group inherit the group's permissions (role definition)
* Roles in Azure are a collection of actions that a user can perform
    * Each Azure resource will have a set number of actions that can be performed on it such as starting a virtual machine or updating a database
    * We can use RBAC to define particular roles where a user of that role can perform a set of actions such as a database operator being able to update, create, delete and scale a database
    * In Azure, these collection of actions are known as **role definitions **
* Built-in roles are predefined roles that cover common roles such as:
    * Administrators (Owner)
        * Can do everything
    * Contributors
        * Can do everything except change access
    * Readers 
        * Can only read
* Custom roles are fine-tuned and can have customised role definitions
* In addition to role definitions, a role is assigned a scope
    * Scopes are a collection of resources
    * All resources will inherit the role given by the scope
    * If the scope is a management group (the highest scope) then all resources underneath will have the same role
* Roles should apply the following standards
    * Least privilege access (give enough permissions to do the job)
    * Role segregation 
    * Audit roles regularly

Control Plane



* The control plane is the ARM (Azure Resource Manager)
* We use the control plane to manage resources
    * Create new ones
    * Delete resources
    * Modify permissions
    * Grant access
* We can interact with the ARM using:
    * The Azure Portal
    * Command line interface / Powershell
    * API
* The control plane can be restricted by
    * RBAC
    * Azure Policy
    * Resource locking
    * Activity Log

Data Plane



* The data plane is where data is stored
    * Blobs in object storage
    * Database tables in databases
    * Secrets in the key vault
* Data plane objects have endpoints where we can access the data without  using ARM
    * This could be a URL such as blob.boomy.windows.net
    * This could be using Azure active directory (Entra ID)
* If a user has the right permissions on the control plane, they  can access the data plane despite the data plane being separate from the control plane
* Data plane objects can be restricted by
    * RBAC
    * Specific Logs

(Hierarchical) Scope in Azure



* Management Group
    * Top of the scope hierarchy 
    * Consists of a collection of subscriptions
    * Management groups are optional
    * Each tenant can consist of multiple management groups
    * Root management group is the very top of the hierarchy chain; non-root management groups can be children of root management group (and only have one parent) but have many child management groups
    * When an organisation has multiple subscriptions, management groups can be useful to group subscriptions (such as an "Asia management group")
* Subscription 
    * A collection of Azure resource groups
        * A resource group can only belong to one subscription 
        * A resource group needs to be attached to a subscription 
        * Subscriptions are billing entities (billing is attached to subscriptions only)
        * We can apply access policies to subscriptions using RBAC (and these policies will apply to children resource groups and resources)
    * Normally subscriptions are used to separate billing (though this can be done with tags) but it can also be used to separate a collection of resource groups from one another
    * Normally we designate subscriptions to different departments 
* Resource group
    * A collection of resources
    * Resource groups are assigned a region but the region is only storing metadata of the resource group
    * Resources within resource groups:
        * All resources must be in a group and can only belong to one resource group
        * Resources in resource groups can be hosted in multiple regions
        * Resources can interact with other resources outside of its resource group (resource groups do not restrict interactivity between resources)
    * The grouping is arbitrary but usually based off resources that are used to run an application (so a virtual machine + database + disk storage for a website)
        * This makes it easy to delete an 'application' as it will delete all resources within the resource group (lifecycle allocation)
        * Grouping also facilitates access control (RBAC)
* Resource
    * A single service in Azure such as a virtual machine or database
    * Resources are usually assigned to a region
    * Resources usually have a cost involved (some are free like networking)
    * Resources also need to be designated a name

Defence in Depth



* Defence in depth is the cybersecurity practice of protecting our data using multiple layers 
    * This requires the hacker to circumvent multiple security of layers in order to access sensitive data
* There are 7 layers when protecting data on computers
    * Physical security
        * Prohibit unauthorised access to the physical location of the data centre
    * Identity and access
        * Only grant account access when it's needed and avoid providing open access to users unless strictly required
    * Perimeter
        * Network-based attack protection such as:
            * DDoS protection
            * Firewalls / network security groups
        * Remove public access (public IP)
        * Use Azure Bastion to access VMs without using public internet
    * Network
        * Secure connectivity between resources
        * Utilise subnets to isolate groups of virtual machines / network resources
        * Utilise network peering to facilitate VPN communication without utilising the public internet
        * Implement hybrid networking
    * Compute
        * Protecting virtual machines from vulnerabilities
            * Maintaining updates to operating systems
            * Endpoint monitoring (anti-malware)
        * Protect access to VMs
            * Using secure logins / keys
            * Use RBAC and Entra ID (Azure Active Directory) authentication
    * Application
        * Patch application vulnerabilities
        * Prevent access to secrets
        * Utilise single sign-on (SSO)
        * Enforce SSL encryption for communication 
    * Data
        * Limit access to data directly using RBAC or preventing anonymous access or using private endpoints
        * Encrypt disks 
        * Use immutable blob storage which prevents files or data being overwritten
        * Access keys to prevent access to data without authentication
* For users, there are specific layers that protect them
    * Passwords
    * Multi-factor authentication
    * Conditional access

Azure Resource Manager (ARM)



* ARM is a service that is used to create and manage all resources in Azure
    * Every service in Azure is connected to ARM
    * Many 'resources' such a virtual machine have multiple 'components' (such as a network interface or disk storage) which are all considered 'resources'
    * It includes features such as tags, access control and locks for all resources 
* All our methods of interacting with Azure go through ARM whether that is:
    * Using the web portal
    * Using powershell
    * Using Azure CLI (command line interface)
    * Using APIs	
* ARM can maintain and update resources using JSON files (known as ARM Templates)
    * These JSON files declares to ARM what properties a resource is to have (such as the type of resource or the name of the resource)
        * ARM templates are declarative
        * ARM templates are repeatable
        * ARM templates are modular
        * ARM templates are testable using specialised software
        * ARM templates are exportable
            * We can click a resource in ARM and export it as a JSON file which we can then use to reproduce the same resource
            * When deploying ARM templates, ARM will compare the difference between the current state and the state declared by the ARM template and make changes accordingly; sometimes this may not even require re-deployment of the resource (such as a change to the locality of an availability zone)
    * BICEP files are more human-readable version of these JSON files which are compiled into JSON by ARM

Azure Portal



* The Azure portal is the web-based interface that shows all resources on Azure
    * There is a search bar for searching various resources as well as documentation
    * The left navigation bar shows commonly used or recommended resources
    * The home pages also shows commonly used or recommended resources
* The Azure portal can be customised to show different bits of information as well as differing the layout and UI elements (such as dark mode)

Azure Command Line Interface (CLI)



* Azure CLI is a command line tool (a program) that interacts with Azure resource manager (ARM) 
    * It can be run in bash and we can use bash to automate tasks using Azure resources (but it is not bash replacement)
    * It uses UNIX-style command language (similar to bash)
    * It can be run in the Azure Cloud Shell (though other command line tools such as powershell or bash can be used too) which runs off the web browser
    * It can be installed on various operating systems
* Azure CLI allows users to create powershell or bash shell scripts that **automate **resource management on Azure
* Can be installed on:
    * Windows
    * MacOS (Homebrew)
    * Linux
    * Docker container
    * Cloud Shell

Azure Powershell



* Powershell is Windows' command line shell offering 
    * Powershell can run powershell scripts 
    * Powershell programming language can also be used for crafting a configuration management framework (using desired state configurations)
* Powershell can be accessed using:
    * Azure Cloud Shell
    * As a program running on an operating system
        * Linux
        * Windows (pre-installed)
        * MacOS
* Powershell programming language / command line usage is based of a verb-noun pairs to perform commands which is somewhat intuitive

<table>
  <tr>
   <td>
   </td>
   <td>
Azure CLI
   </td>
   <td>Azure Powershell
   </td>
  </tr>
  <tr>
   <td>Syntax
   </td>
   <td>Terse (short)
   </td>
   <td>Verbose (descriptive)
   </td>
  </tr>
  <tr>
   <td>Shell compatibility
   </td>
   <td>Powershell only
   </td>
   <td>Any command line interface
   </td>
  </tr>
  <tr>
   <td>Language
   </td>
   <td>Uses own proprietary programming language similar to bash
   </td>
   <td>Uses Powershell programming language
   </td>
  </tr>
  <tr>
   <td>Programming model
   </td>
   <td>Functional 
   </td>
   <td>Kind of object-orientated
   </td>
  </tr>
  <tr>
   <td>Installation
   </td>
   <td>An executable
   </td>
   <td>Module of powershell
   </td>
  </tr>
</table>


Azure Cloud Shell



* Azure cloud shell is a command line interface that runs off the web browser (via Azure Portal) 
    * Azure cloud shell can technically also be run through Windows Powershell 
    * This will require login details to Azure
* It has some advantages over using a dedicated command line interface tool on a client computer:
    * Automatically authenticates with Azure
    * Provides two different shell options (bash or powershell)
    * Integrates Azure powershell and Azure CLI out of the box
        * No need to install Azure CLI
        * Not need to install Azure powershell
    * Directly accesses Azure storage resources

Azure Cost Management



* Azure provides a collection of tools for controlling the budget for the resources currently used in Azure such as
    * Predicting bills
    * Optimise the best way to use resources to minimise cost
    * Reduce waste and thus reduce the cost spent on underutilised or unused resources
* Some actual tools included:
    * Azure Cost Management and Billing
    * Azure Advisor
    * Azure Budgets
* If you want to see a predicted cost for resources that have not been deployed then use Azure Pricing Calculator

Azure Support



* Basic Support
    * Default support plan provided to all Azure customers
    * Includes access to:
        * Online documentation
        * Forums and community support	
    * Suitable for non-production environments and users who prefer to troubleshoot issues independently.
* Developer Support
    * Includes all basic tier support options as well as:
        * Technical support during business hours via email
    * Suitable for developers and users working with testing environments
* Standard Support
    * Includes all developer tier support options as well as:
        * 24 x 7 technical support during business hours via email or phone
        * Response times will vary based on severity
        * Architecture reviews
        * Best practice analyses and recommendations
    * Suitable for developers and users working with production workloads
* Professional Direct Support
    * Includes all standard support tier options as well as
        * A dedicated technical account manager
        * Monthly health checks
        * Enhances SLAs (service level agreements):
    * Suitable for businesses with mission-critical workloads and complex architecture

Subscriptions and billing



* Subscriptions are agreements with Microsoft which the user to access cloud services (for money)
* The billing cycle can differ:
    * Pay as you go
    * Enterprise Agreement (discounted rate for using a minimum level of usage)
    * Azure Dev/Test billing (reduced rates for non-production workloads)
    * Free account (restricted usage at no cost)
* The pricing may be reduced in certain circumstances:
    * Reserved instances (discounted rate for committing to services for a set period of time such as a 1 or 3 year time period)
    * Spot Pricing (use spare capacity at a discounted rate but uptime is not guaranteed)
    * Windows Server licence discount (Azure Hybrid Benefit provides a discount if users have an on-premise Window Server)
* Some examples on the pricing structure of different resources 
    * Virtual Machines
        * Pay more for more computing power / RAM / storage / operating system
        * Pay more the longer the virtual machine is operating
    * Storage
        * Pay more for higher redundancy
        * Pay more for more capacity per month 
        * Cost dependent on storage type
            * Archive storage is the cheapest (and least accessible)
            * Hot (fast) storage is more expensive
    * Data transfer
        * Inbound data is usually free
        * Outbound data usually has a cost involved
            * Network bandwidth for a web server
            * Transferring data between availability zones
    * Databases
        * Pay more for more capacity
        * Pay more for faster database speeds
        * Pay more for more transactions
* Subscriptions can also be used to group multiple resource groups together and separate resource groups from one another (for access or billing or usage reasons)
    * A common way to use subscriptions is to separate them by departments (such as a development subscription and a marketing subscription)

Azure Price Calculator



* The price calculator provides an interface that shows all Azure resources and calculates pricing based on your selection
* The Azure price calculator is its own separate website (not in Azure portal) 
    * Users can select product categories and then use the product picker to select specific resources (such as compute → virtual machine) to get an estimate of the costs involved for using that specific resource
* Price estimation requires users to consider:
    * Type of resource needed
    * Scale of the resource needed
    * Flexibility in requirements (how fast does the virtual machine need to be)
    * Immutable requirements (this service must be hosted in Europe)
* Some features of the calculator
    * Select various settings of a particular resource
        * Region
        * Type (such as operating system for a virtual machine)
        * Tier (how premium the offering is)
        * Instance (the specific resource details such as single core 1GB ram VM)
        * Saving options
        * Add-ons (such as storage for a VM or database)
    * Export costs into CSV or spreadsheets
* Common mistakes when using price calculator
    * Over Estimating resource needs
    * Forgetting bandwidth (data transfer costs)
    * Ignoring price variation based on location
    * Forgetting discounts
* Actions to improve cost estimates
    * Update usage patterns regularly to get more up-to-date estimates
    * Factor in future growth
    * Use Azure pricing examples such as the cost to run a web server

Azure Total Cost of Ownership Calculator



* This calculator compares the cost of using Azure vs. using an on-premise server
* It considers various aspects such as
    * Hardware maintenance costs
    * Staff costs
    * Licencing cost
    * Cost of utilities
    * Cost of downtime
* It requires:
    * Current on-premise workloads (use inventory tools to gather data on all components of the current on-premise setup)
    * Projecting growth and accommodating for it in calculations
    * Adjust aspects specific to your setup such as redundancy, location and applicable discounts

Azure Cost and Billing Management Tool



* This tool has four main components
    * Cost Analysis: breaks down costs to understand how money is being spent
    * Budget: Set a threshold for how much you want to spend on Azure and set limits
        * We can set budgets at a subscription, resource group or resource level
    * Cost Alerts: Get an alert when spending reaches a certain threshold 
        * We can set a threshold for an alert (such as 50% of the budget)
        * We can send a notification (via email or portal notification)
        * We can perform an automated action such as shutdown a VM
    * Azure Advisor: Gives suggestions based on usage patterns on how to reduce costs
        * This service is free and accessible via the portal or via API
        * It also provides recommendations on security, reliability, 'operational excellence' (best practices) and performance 
* This tool can be accessed from search bar where it will show costs associated with the main account (or subscription if you are not root administrator) or it can be accessed on the navigation bar when selecting a specific resource (the cost analysis will then only be performed on the selected resource)
* Another way to track spending is the use of tags

Tags



* Tags are key-value pairs that form part of an entity's metadata
* Just like resource locks, they can be applied to:
    * Subscriptions
    * Resource groups
    * Resources
* Tag properties
    * Tags are not inherited
    * They are key-value pairs (owner: Kevin)
    * The key can be shared which can help in identifying resources
        * If we use the owner tag we can find all resources that have an 'owner'
        * We can then find out all resources owned by Kevin
* Tags are used for various reason
    * Cost tracking
    * Security purposes (sensitive data)
    * Resource management	
* Azure Policy can be used to enforce tagging or automatically tag resources
    * If tagging is enforced but not complied with, the new resource will not be created
    * Tag inheritance can only occur with a Azure Policy which can tag all children entities

Azure Policy



* Azure policy is a service that sets rules and checks on resources that comply with governance rules set by the organisation
    * Without policies, users with permissions could do whatever they want within their set permissions and this may break the budget or break regulatory rules 
    * We could have an individual (operations team) manually check each request but this is too labour-intensive and slow
    * We could use Azure policy to customise some 'guardrails' on how users provision resources in Azure and enforce these rules for organisations
* Azure policies can be set to different scopes (management groups / subscriptions / resource groups / individual resources) and they are inherited (a policy on a subscription will apply to child resource groups and resources)
* Azure policies are written in JSON 
* A collection of Azure policies is known as an initiative
* Azure policies have definitions made up of two components
    * A condition
    * An effect
        * Audit (track how often a policy is met/unmet) 
        * Deny (block an action if it doesn't meet a criteria)
        * Append (if something is not there, then append this)
        * Modify (if condition is met, modify this)
        * Exists (if something is there, do this)
* Microsoft Azure comes with a lot of in-built policies and initiatives

Resource Locks



* Resource locks are another way to restrict the usage of a resource outside of RBAC
* We can lock subscriptions, resource groups and resources and they are inherited
* We can apply a resource lock via Azure Portal, Azure CLI or Azure Powershell
* Locks  can be automated (only apply in response to an event or during certain times)
* Only owners can lock or unlock resources (or user access administrator)
* Locks can either 'cannot delete' (delete lock) or 'cannot delete or modify' (read-only)
* Resource locks apply on the control plane (Azure Resource Manager) 
    * This means we cannot modify permissions or modify data using Azure Resource Manager
    * But it does not prevent interactions with the resource on the data plane 
    * So an application that is accessing data within a resource can still do so if its accessing it without using ARM (such as using a REST API)
* The purpose of resource locks are mainly used to prevent accidents or performing maintenance or preventing changes to critical resources 

Microsoft Purview 



* Purview gives an overall view of the data 
    * Data can be stored in:
        * Microsoft 365 / OneDrive
        * Azure (Blob) Storage
        * AWS S3 Bucket
        * PowerBI (data analytics tool)
        * Other software providers
    * Purview gives a summary of:
        * Where is the data stored
        * Who has access to this data
        * Is this data sensitive
    * Purview comes with a free and enterprise editions
* Functions of Purview 
    * Scan data and create a data map 
    * Classify the data and label it
    * Provide insights (data lineage which is the history of transformation and transportation of a piece of data)
* With this data we can:
    * Create a catalogue (report) of the data
    * We can share the data (read-only) for auditing purposes / analysis 
    * We can create policies that apply to this data
    * We can give 'estate insights' of where data is and assess risk 

Microsoft Defender for Cloud (Azure Security Centre)



* It provides a range of security services for not only Azure services but third-party cloud vendors (such as AWS resources or Github repositories) and on-premise services
* It gives an overview of the security of managed resources
    * A secure score
        * Enabling multi-factor authentication will increase the score greatly
        * Applying system updates will increase the score
        * Secure network ports will increase the score
    * Recommendations
        * Some recommendations will provide a one-click solution (quick fix)
        * You can also 'exempt' the recommendation if using a third-party service to remediate the 'security issue'
* It can assess the security status of your subscription / resources against various regulatory compliance protocols
* It can provide alerts which can then trigger actions or provide notifications to administrators (such as when an unknown login occurred)
* Enhanced security (costs money) can provide additional features such as
    * Just in time VM access (open network ports when a request is made by a user instead of leaving the network port always open)
    * Adaptive application control 
    * Regulatory compliance reports
    * Threat protection (anti-virus)

Azure Sentinel



* Azure Sentinel is the 'response' to security events
* It can connect to many different resource types using 'data connectors'
    * Each data connector will cost money
* It uses machine learning from various logs and determine if a threat is occurring
* We can define rules (analytics) based on the Kusto Query Language (KQL)
    * These rules are used to analyse logs to determine if a security issue
    * When such issue arises, we can either send an alert or create an incident
    * We can also use pre-made templates as well 
    * An example rule template is detection of a brute force attack
* We can create an alert which can run a **playbook (Azure logic app)** to respond to an event
    * We can create a logic app ourselves
    * There is a large repository we pre-made logic apps we can use such as "block an IP" or "send a message"
* We can create Azure Monitor Workbooks (using KQL or using templates) which can create a dashboard that shows various metrics relating to security

Azure Monitor 



* Azure monitor provides a central location for all logs
    * Azure active directory (Entra ID) audit and sign-in logs
    * Subscription activity logs (normally saved for 90 days) and service health
    * Activity logs (such as actions performed in Azure portal or ARM)
    * Resource metrics (telemetry)
    * Resource logs (needs to be enabled)
* We can save these logs to various locations
    * Azure storage (only for storage not for analysis)
    * Event hub (publish / subscribe service) 
    * Log analytic workspace (an Azure Monitor service)
* Purpose of Azure monitor
    * Examine resource metrics (such as how much storage is being used over time)
    * Produce alerts (alert rules) based on log information and trigger actions (action rules) 
        * A custom alert could be CPU usage above a certain percentage
        * An example action would be calling an Azure function or send an email/SMS
    * Azure monitor can be used:
        * Proactive (anticipate problems before they occur)
        * Reactive (respond to events)
* We can perform actions in response to particular events
    * We create action groups which are a collection of actions that are performed when an alert is triggered

Azure Event Grid



* Azure Event Grid is a service that can respond to events
* Events can be Azure-native or third-party
    * Blob Storage
    * Azure Functions
    * Azure IoT Hub (MQTT protocol)
    * Azure Kubernetes Service (AKS)
* Event Grid is a serverless service
* We can set event handlers that respond to events
    * Webhooks
        * Azure Automation runbook
        * Logic Apps
    * Azure functions
    * Feed data into Event Hubs

Azure Event Hubs



* Azure Event Hubs is a service that processes telemetry data from events or devices
* The data is normally from
    * IoT devices
    * Applications
* Functions
    * Stores data for a set period of time
    * Can perform batch operations on data

Azure IoT Hub



* The internet of things (IoT) is the idea of ongoing communication between internet-connected devices and a cloud service
    * Usually this data is telemetry data (such as sensor data)
    * We can also send signals to devices to perform various actions
    * We can also send updates to devices (such as firmware updates)
* Azure IoT Hub facilitate identification, authentication and communication of various IoT devices
    * Azure IoT Hub will create a device twin and it can interact with IoT Devices such as
        * Push firmwares
        * Collect telemetry
        * Request telemetry data
        * Request an action
    * Azure IoT Hub provides an SDK to integrate IoT devices (by creating our own application) with IoT Hub
* Azure IoT Central is a software as a service solution that incorporates IoT Hub that includes some pre-built templates such as:
    * Applications
    * Device templates
    * Device emulation
    * Common industry scenarios

Azure Advisor



* Azure advisor provides suggestions based on best practices
    * Cost optimisation
        * Downsize resources
        * Remove idle resources
        * Consider reserved instances for resources that are used a lot and likely to be continued to be used in the future
    * Performance-related improvements
        * Upsize resources
        * Upgrade SDK
    * Reliability improvements
        * Redundancy
        * "Soft delete" to prevent accidental deletion
    * Security issues
        * Multi-factor authentication
        * Vulnerability settings (exposed ports)
    * "Operational excellence"
        * Service health
        * Subscription limits
* Each recommendation has a:
    * Impact
    * Description
    * Benefit
    * Affected resource
* Some recommendations can be implemented by clicking a few buttons
    * We can also postpone recommendations
    * We can dismiss them as well

Azure Automation 



* Automation is a tool that automates stuff in Azure
    * Process automation
        * Automate tasks using python, powershell or powershell workflow
        * Tasks can be triggered by schedules or events
        * Tasks can run on Azure or on-premise computers
    * Update management
        * Update Windows or Linux systems automatically 
    * Configuration management
        * Apply desired state configuration (DSC) to virtual machines
* Azure Automation can perform similar actions to Azure Functions (normally triggered by a web API call) or Azure Logic Apps (a GUI service)

Azure Applications Insights



* Application insights provides various functions for our applications
    * Metrics
        * Provides a live metrics feed
        * Can gather performance and health metrics
            * Availability
            * Failures
            * Performance (CPU usage)
    * Alerts
        * Prompt alerts based on metrics or event data
    * Application map
        * Provides a visual representation of the components of the application
        * Can be useful for identifying failure hotspots or performance bottlenecks
    * Profiler
        * Captures performance traces of our applications
        * Can be useful for identifying slow operations or unoptimised code
    * Usage analytics
        * User flows (the path that users navigate)
        * Session details (how long a user spends on a part of the application) 
        * Retention (how often do users use the application over time)
* Application insights can collect data at various points
    * Client-side
    * Application-side
    * Dependencies
        * Web server
        * Databases
* Applications insights can be enabled by:
    * Using Azure App service and enabling it in Azure Portal (basic data collection)
    * Incorporating the Application insight SDK into our application code using a connection string / instrumentation key
        * Node.js
        * Python
        * Java
        * .NET

Azure Service Health



* Service Health is a tool that gives an overview of the health of services, subscriptions, resources and regions
* "Health" is defined as an entity that is running without issues, performing as expected 
* "Unhealthy" is defined as an entity that is:
    * Misconfiguration
    * Bugs in software code
    * Hardware failure / unexpected outage
    * Performance issues (not enough RAM or CPU)
    * Network issues (packet loss / high latency / 'lag' / DNS resolution problems / traffic spikes)
    * Security breaches (unauthorised access
    * External dependency failure (third-party service goes down)
* Any unhealthy service will have:
    * A summary of the problem
    * Any updates
    * An a root cause analysis (happens after a few days)
* Azure Service Health can provide information about:
    * Planned maintenance
    * Incidents 
    * Health of various resources 
* Alerts can be sent when the health of a service is affected

Azure Blueprints



* Azure blueprints is a template of 'actions' that we can apply to different subscriptions
    * Resource groups
    * ARM templates
    * RBAC
    * Policy
* Blueprints can be 'locked':
    * Do not delete		Users cannot delete 
    * Read-only		Users cannot delete or modify
    * Unlocked		Blueprint is just a 'default' setting that can be modified
* Subscription owners cannot break the lock set by a blueprint unless they assign the blueprint 
* Blueprints can be updated 
* The main use of blueprints is:
    * Collection of various 'templates' such as ARM templates and policies
    * Unlike ARM templates which cannot monitor if the resource specifications match the template, blueprints can track this
    * Blueprints can be deployed onto multiple subscriptions whereas ARM templates can only be deployed into one subscription
    * Blueprints are stored on Azure (ARM Templates are just JSON files which are not natively stored in Azure)
    * 

Virtual Machines (Azure Virtual Machines)



* A form of infrastructure as a service
* Virtual machine properties
    * CPU
    * Memory
    * Disk
    * Networking (free)
        * Network interface card
        * Virtual network
        * Network Security Group (open port)
    * Network Controls (Firewall)
    * IP address (not free)
    * Operating System (Linux or Windows)
* All virtual machines needs to be deployed onto a virtual network (VNet)
    * A VNet includes at least one subnet
    * All VMs are given a public and private IP address (private is mandatory)
* Different virtual machines have different 'sizes' which are different CPU / RAM combinations
    * These VMs are grouped into series 
    * The B and D series are balanced CPU to memory ratio
    * The F series are heavy on CPU which is ideal for high traffic web servers, batch processes and application servers
    * The E series are heavy on RAM which is ideal for relational databases and caching
    * The L series is a storage optimised option with high disk throughput and ideal for I/O intensive operations such as NoSQL databases
    * The N series have dedicated GPUs targeted at graphics (video rendering / editing or AI model training)
* Pricing varies depending on the series
    * Compute component (CPU/RAM) is priced per minute
        * Powerful CPU/RAM combos cost more
        * Users can 'pause' their VM instance to freeze their costs
    * Disk is priced by GB per month
        * Faster disks cost more
        * Bigger capacity disks cost more
        * Note bigger capacity disks normally have faster transfer speeds
    * Operating system are priced per minute
        * Applies for Red Hat Linux and Windows
        * Like Compute, pricing is pay-as-you and can be 'frozen'
    * IP address (networking) is charged by the hour
        * Pricing depends on the SKU
            * Static IP addresses are more expensive 
            * Dynamic IP addresses are 'lost' when VM is paused/terminated
* Benefits of using virtual machines
    * Control
    * Application compatibility (if it runs on a computer, it will run on a VM)
    * Ease of transfer (easy to move existing infrastructure to the cloud with infrastructure 
    * Useful for testing and development environments 
    * Useful to extend existing data centre capabilities
* Things to be wary of when using virtual machines
    * More management
        * Operating system updates / patches
        * User control
        * Software environment
        * Configuration management
    * Higher costs
    * More complexity when scaling
* Connecting to virtual machines
    * SSH for linux (port 22)
        * Can use Azure CLI (command line interface)
        * Can use any other shell via SSH
    * RDP (remote desktop protocol - port 3389)
    * Ideally these ports should not be exposed to the public internet in production 

Virtual Machine Scale Sets



* Scale sets are a set of identical virtual machines which are used for scaling applications and distributing the load onto many virtual machine instances
    * This distribution is handled by a load balancer
    * This is useful for when there is too much load/traffic funnelled into a single virtual machine
* VM scale sets are designed to provide horizontal scaling
    * VM sets are placed behind a load balancer
        * The domain is usually set to point to the load balancer
        * The load balancer will then pick a VM to send the customer to
        * Since all VMs are the same, the customer will always get the same response
    * They will increase or decrease VM count based on automatic policies or manually set by the administrator
* Benefits of VM scale sets
    * Load balancing
    * High availability
        * If one instance of a VM fails, the other VMs in the set can tae over
        * VMs can be deployed in different zones to facilitate zone redundancy
    * Auto-scaling
    * Large scale
        * We can implement up to 1000 VMs in a set
        * This allows organisations to expand 
    * No extra cost (for implementing scale sets)
        * Note if you do use more VMs then you pay for them
        * But the cost of implementing VM sets is 'free'
* Configuring VM scale sets
    * We can set a **baseline image **which will be imaged onto all VMs
    * We can alternatively create a **startup configuration script** which is run on boot and is designed to create the instructions to create the same environment in all VMs
    * We can employ both strategies in creation of VMs in scale sets

Availability sets



* Availability sets provides high availability for static VMs within a single data centre
* Differences between scale sets and availability sets:
    * Availability sets: non-identical VMs		Scale sets: Identical VMs
    * Availability sets: no auto-scaling		Scale sets: Designed to auto-scale
    * Availability sets: single data centre / zone	Scale sets: Can multi-zone
    * Availability sets: free				Scale sets: Cost dependent on VMs
    * Availability sets: good for unique VMs that don't need auto-scaling
        * An example would be a website with different components hosted on different servers
* With availability sets, the VMs are placed in different fault and update domains
    * A fault domain is a group that is contained within a server rack with common power source and network switch
        * Normally multiple virtual machines are hosted on bare metal machines that are stacked in 'server racks'
    * An update domain is a group of bare metal machines that undergo the same maintenance cycle
        * When maintenance occurs (such as OS updating), a group of servers will be put offline for a period of time
        * Update domains are not dependent on physical location 
* The idea of availability sets is to give some control on where VMs are located
    * VMs will be put on hypervisors with separate maintenance windows (update domain)
    * VMs will be put on different server racks (fault domains)
* Availability sets allow for improved availability to overcome the problem of:
    * A server rack losing power or connectivity
    * Maintenance period affecting multiple VMs simultaneously
* Availability set limitations
    * Maximum of 3 fault domains
    * Maximum of 20 update domains

Azure Virtual Desktop



* A services that provides virtualized Windows desktops and apps 
    * This provides a virtual desktop interface
    * It is accessible from any device (with a web browser)
    * It separates OS, data and applications from the client's hardware
* The use case of Azure virtual desktop
    * Better secure data by keeping it on the cloud instead of client's hardware 
        * This means client's hardware does not store sensitive data
    * Reduce IT management overhead of multiple client desktops 
        * Licencing is streamlined since only the virtual host requires licensing
        * Updates and settings to applications are all handled on Azure and not on the client's device
    * Improves consistency regardless of client hardware since the operating system and application is hosted on the  cloud instead of the client's hardware
        * Most devices will be able to access the virtual desktop
        * Can also access using a web browser
    * Scalability since the operating system and application is hosted on the cloud and not an on-premise server or on client hardware
        * We can add more VMs as needed
        * Each VM can host multiple clients
* A virtual desktop consists of:
    * Applications 
    * Configuration / access / diagnostic services
    * Some virtual machines to power everything 
* Applications of virtual desktop
    * Enables remote work
    * Companies do not need to provision hardware to employees (they use existing hardware that they own)
    * Keeps sensitive data on the cloud and not on the user's machine
        * Reduced risk of data breaches (such as the user's device getting stolen and resulting in a data leak)
        * Simplifies compliance such as privacy laws in healthcare settings

Azure App Services



* A form of platform as a service which provides fully managed applications with minimal management required by the end user / administrator
* Using App Services (over IaaS) means that administrators don't need to worry about:
    * Operating systems (configuration / updates)
    * Hosting web server applications (NGINX or Apache)
    * Network management
    * Disk management
    * Load balancers
        * Scaling is automatic
        * Availability is maintained by Azure and kept very high
* The main use of app services:
    * Hosting web apps (websites)
        * Most programming languages are supported (.NET, Python, Node.js)
        * Also capable of deploying static web apps (HTML / CSS)
    * Deploy containers
    * WebJobs (background tasks for application logic)
    * API Apps
        * Host REST-based API
    * Backend for mobile apps
        * Authentication
        * Push notifications 
        * Store mobile app data
* Properties of App services
    * Unique name (unique to **everyone**)
    * Publish method
        * Code
        * Static web app
        * Container 
    * Service plan
        * Performance
        * Scaling
        * Disk space
* How to host your application using App service
    * Connect to GitHub repository
    * Connect to third-party repositories
        * TBitBucket
        * Local Git
        * Azure Repos
    * Connect manually using Git
* Azure App Service supports continuous deployment for rapid iteration

Azure Functions



* A special subset of platform as a service (function as a service)
* Azure functions are 'serverless' event-driven code execution
    * No VMs to manage
    * Code execution only occurs when an event occurs and runs once
    * Normally triggered by a web API or a web address (URL)
* Some use cases of Azure functions
    * Processing an upload (such as resizing an image)
    * Process messages
    * Transform data
    * Scheduled tasks
    * Authentication or payment service
    * Chatbots
    * Internet of Things (turn the smart lightbulb on)
* Benefits of Azure functions
    * Run as required; saves money as only paying for usage
    * Resilience; if the function fails it doesn't affect anything else
    * Scalability; can scale up or scale down to zero 
    * No infrastructure management required

Containers



* Containers is an application that is a package that bundles in files, configurations and dependencies that are necessary to run on a given piece of hardware
    * The operating system is omitted
    * For example, a website container may consist of:
        * Script (HTML/CSS/Javascript code)
        * Images
        * Libraries
        * Web server (like Apache)
    * Containers are packaged such that they can be distributed to any server and run without any additional software
    * Containers will share the host/server operating system so are much more efficient that having multiple virtual machines on a server
* Benefits of containers
    * Less overhead (no operating system)
    * Portable (can be easily made to run on different hardware / operative systems)
    * Comes with built-in dependencies (so no need to worry about installing them on the operating system)
    * Efficiency and scalability; easy to run another container instance
    * Consistency (containers will run the same on any hardware)
* Some disadvantages of containers
    * Applications wrapped into containers have to have different versions to work with different operating systems / computer architecture
    * If the operating system crashes, all containers will crash

Azure Container Instances (ACI)



* Simple and cheapest option for running containers
* Containers are deployed on demand
* Ideal for short-lived simple workloads
* Cannot scale (only one containers)
* No load balancing

Azure Kubernetes Service (AKS)



* Kubernetes is an open-source container orchestration tool
    * It can manage many high-volume and complex containers
    * It offers a lot of control and customisation
* AKS has built in automatic scaling, load balancing and failover (ability to switch to a working service when a failure occurs)
* AKS is more complex and more expensive than ACI

Azure Container Apps



* A system to deploy containers that is a bit simpler than Kubernetes but has a lot of the features that Kubernetes offers such as:
    * Scalability (auto-scaling enabled)
    * Severless
* It has less features than Kubernetes
    * No access to Kubernetes API
    * Less customisable

Other methods to run containers



* Virtual Machines (requires installing Podman or Docker)
* Azure App Service
* Azure Functions

Azure Virtual Network (VNet)



* A virtual network is a isolate private network for VMs to reside in
* Each VM is given a private IP (10.0.X.Y)
* Each VM is given by default a public IP but this is optional
* Public IPs can be dynamic or static; dynamic IPs change when the VM is reallocated
    * Dynamic IP is cheaper and users are only charged when the VM is in use
    * Static IP is better for anything that requires consistency but is more expensive and incurs costs even if the attached VM is not active
* Each VNet is bound to a region
    * All VMs in a VNet must be in the same region
* Each VNet belongs to just one subscription (but subscriptions can have multiple VNets)
* The benefits of using a VNet
    * Software defined networking simplifies networking as no 'physical cables' need to be attached to each networking device 
    * Very easy to scale using virtual networks
        * Can easy to make new networks easily
        * Can expand more IP addresses easily with some configuration tweaks
    * High availability via the use of
        * Load balancers
        * Peering VNets
        * VPN gateway
    * Easy to isolate networks using subnets and network security groups
* VNets can connect to many different entities
    * The public internet (using IPv4 or IPv6 public IP addresses)
    * Other VNets (intra-VNet and VNet peering)
    * Managed services (such as services on Azure)
    * Hybrid networking (connect to other cloud networks or on-premise networks)

Network basics



* Each local network has an address space which is the range of usable local IP
    * This is usually designated 10.0.X.X/16 in Azure
    * We use CIDR (Classless Inter-Domain Routing) to denote subnets within IP address ranges
* Within each address space we can allocate subnets
    * For example subnet A may be 10.0.1.0 - 10.0.1.256 (10.0.1.0/24)
    * Subnets are useful for:
        * Resource grouping (for example all devices on the subnet may be web servers)
        * Address allocation 
        * Subnet security using security groups
* Private IPs are usually within a set range and only accessibly within a local network
    * 10.0.0.0/8
    * 172.16.0.0/12
    * 192.168.0.0/16

Network security groups (NSG)



* Network security groups are filters that can block malicious traffic to your VMs or subnets
* They are a free service
* They provide granular (fine) rules for network controlled
    * Inbound or outbound traffic restrictions
    * Block traffic based on
        * TCP / UDP ports
        * ICMP (Internet Control Message Protocol - pings)
        * Allowed sources / destinations (allow parts of the internet to have access)
    * An example of a use of NSG is allowing RDP port (TCP 3389) to be open only to IP addresses from within the organisation

Azure Firewall



* A filtering service just like NSG but with more advanced features such as
    * Centralised traffic control for multiple VNets
    * Threat intelligence (provides alerts to suspicious activity)
    * Ability to block based on domain
    * URL filtering
    * DNS proxy
    * Can connect and filter on-premise networks
* Azure Firewall is expensive so its mainly used by enterprises

Azure Bastion



* Allows secure SSH / RDP access to private VMs 
* Normal VMs without a public IP are inaccessible remotely however with the use of Azure Bastion which acts as a jump server and allows remote connections to private VMs
* Azure Bastion is deployed onto a VNet with a specific "AzureBastionSubnet" specified (when creating a subnet we can select a subnet template and AzureBastionSubnet is an option we can select from)
* This service is fully managed and is a paid service

VNet peering (Virtual network peering)



* Virtual network peering allows private connectivity between Azure VNets using Azure private network 
    * This traffic is not exposed to the private internet (uses Microsoft's private internet service)
    * It allows VNets to access other Vnets on:
        * Different availability zones
        * Different regions
        * Different tenants (owners)
* The benefits of peering
    * It's fast (low latency)
    * It's secure (no public internet access)
    * Allows for custom network security groups and custom routes
* An alternative way to connect to VNets in different regions is to use a VPN

DNS



* DNS (Domain name system) is a system of giving public IPs a 'domain name'
* DNS servers have a database that store this information
* Connection requests from clients is 'resolved' by a DNS host or server which will convert a domain name into a public IP 
* DNS can work on public or private networks
    * Public networks uses a public domain registrars to issue domain names and these records (CNAME / A / MX) are saved on authoritative name servers
    * Private DNS servers are usually hosted on the cloud or on-premise hardware and can convert a domain name into a private IP address

Azure DNS Zones



* Azure DNS Zones provides public DNS resolution
* This service allows Azure to convert your domain name into a public IP address
    * We can set DNS records such as A or MX or CNAME
        * A (Address) record is the most common type and maps a domain name to the IP address of the server hosting the domain's website
        * CNAME (Canonical Name) records are used to alias one domain name to another; such as [www.boomyville.duckdns.org](http://www.boomyville.duckdns.org) to boomyville.duckdns.org
        * MX (Mail Exchange) records specify the mail server responsible for receiving email messages on behalf of a domain
        * TXT (Text) records are used to associate arbitrar
    * The benefits of using Azure DNS Zones:
        * Azure has multiple DNS servers hosted all over the world so it can respond faster
        * It integrates with the Azure ecosystem
        * We can use RBAC to control access DNS records
        * We can monitor activity to DNS records
        * We can use resource locks to prevent changes to DNS records

Azure Private DNS Zones



* Allows for the use of domain names to point to private IPs within Azure VNets
* Since this service runs on the private network, it is fast and does not expose anything to the public internet

Hybrid networking



* Hybrid networking is the connection between an external network and a private network using a VPN
* The main use of hybrid networking is the extend the scope of a private network to allow a trusted external network to gain access to it 
* We normally use this type of networking for connecting to:
    * On-premise networks
    * Other cloud networks (AWS or GCP)
    * Other Azure VNets
* When we create a VNet gateway to connect to a third party network using a VPN, we call this  service a **VPN gateway **(opposed to ExpressRoute which doesn't use public internet)
* Azure offers three types of VPNs
    * Site-to-site (network to network) VPN gateway
        * Requires a public facing router on the on-site network to accept external connections and the creation of a **local network gateway **service within the Azure VNet 
        * Connections are encrypted (usually using an IPsec tunnel)
        * Connectivity is done over IPsec (Internet Protocol Security) and IKE (Internet Key Exchange) which are network communication protocols
        * Uses the public internet
    * Point-to-site (network to computer) VPN gateway
        * Allows the Azure network to access an individual computer
        * Mainly used for remote workers
        * Requires configuration of the VPN to be set for point-to-site connectivity
        * Uses the public internet
    * ExpressRoute
        * Connects an on-premise server to the Azure network
        * Uses Microsoft private connection (not the public internet)
        * Is expensive and requires an ISP to facilitate a physical connection from an on-premise server to Microsoft's servers directly
* VPN types
    * Policy-based
        * More backwards compatible (with more devices / networks)
        * Only allows for static routing
            * Network administrators need to manually define static routes and subnets to connect to
            * This involves having preset paths which routers use to send data 
            * Static routing does not support load balancing or scalability but it does provide a predictable environment for networking
        * Cannot be used for point-to-site VPN
        * Only one site can be connected to
    * Route-based
        * Lower compatibility
        * Supports dynamic routing (so routers can determine the fastest way from origin to destination) and this inherently allows for scalability (adding more routers) and load balancing (better availability and reliability)
        * Can be used for point-to-site VPN
        * Many sites can be connected to
* A virtual network gateway is a managed Azure resource hosted within a VNet that acts as an endpoint for external connections to occur
    * It has its own subnet (named GatewaySubnet)
    * Only one virtual network gateway per VNet
    * Each virtual network gateway service has two VMs that facilitate traffic
        * The active-standby configuration means that one VM is running the network tunnel and another VM remains in standby and only takes over if the primary VM loses connectivity or crashes
        * The active-active configuration means two VMs maintain two active network tunnels
            * This requires two public IPs for each VM
            * Provides maximum high availability
            * On-premises router needs to support two network tunnels at the same time

<table>
  <tr>
   <td>
   </td>
   <td>
Peering
   </td>
   <td>VPN
   </td>
  </tr>
  <tr>
   <td>Encryption
   </td>
   <td>No
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td>Public exposure
   </td>
   <td>No
   </td>
   <td>Yes
   </td>
  </tr>
  <tr>
   <td>Speed
   </td>
   <td>Fast
   </td>
   <td>Slower
   </td>
  </tr>
  <tr>
   <td>Bandwidth
   </td>
   <td>High
   </td>
   <td>Limited
   </td>
  </tr>
  <tr>
   <td>Cost
   </td>
   <td>Cheap
   </td>
   <td>Expensive
   </td>
  </tr>
  <tr>
   <td>Configuration
   </td>
   <td>Easy
   </td>
   <td>Complex
   </td>
  </tr>
</table>


Azure ExpressRoute



* A private and dedicated connection to Azure and Microsoft's other cloud services that does not use the internet
    * It can only be used to connect an on-premise network 
    * It requires a physical connection to Microsoft's network
    * This connection is 'leased'
    * This connections normally needs to be facilitated by an ISP or a third-party service provider
    * This connection requires up front costs and takes weeks to months to implement
* We can a connect an on-premise network to:
    * Microsoft Azure services
    * Microsoft Azure virtual gateways
    * Microsoft 365
    * Microsoft Dynamics
* The main benefits to use ExpressRoute
    * Very fast
    * Built-in redundancy

Endpoints



* Endpoints are a unique network address that acts as the destination or arrival gate for network communication
* A public endpoint is a network address or service that enables a resource (normally a PaaS resource) to be connected to via the internet
* This means any data transferred (for example a virtual network to Azure storage) travels along the public internet which may not be ideal for data sensitive applications
* We can secure public endpoints by
    * Using a service endpoint
        * A service endpoint is a service that creates a route for data / traffic to be routed from a virtual network to an Azure resource
        * This service endpoint can be implemented by only allowing traffic from known virtual networks (firewall rule)
        * This option still means an Azure resource has a public IP
        * This option is free but only works within Azure 
    * Using a private endpoint (and turning the public endpoint off)
        * A private endpoint allows an instance of an Azure resource to have its own private IP (virtual network interface) within a virtual network
        * Private endpoints allow for connectivity between Azure resources and virtual networks / on-premise networks using Microsoft's internal network (and not the internet)
        * This private IP needs DNS resolution (can be automatically done by Azure private DNS)
        * This private IP representation of an Azure resource instance will live within a subnet and can be connected by:
            * Other subnets within the virtual network
            * Another virtual network (in a different region) using VPN or peering
            * An on-premise network connecting to the virtual network using ExpressRoute or VPN
        * The use of a private endpoint means the Azure resource instance does not need a public IP to connect to a virtual network and this connection can be turned off
        * Private endpoints have a cost involved and are more complex 

Storage accounts



* Storage accounts is a management layer where we can configure storage:
    * Performance
    * Security and access
    * Provides an unique namespace for all storage objects within the account (each storage resource instance will have its own unique name)
* Different combination of storage resources can be attached to a storage account
    * Blob containers
    * Files
    * Queues
    * Tables
    * Disks
    * Data lakes (used for data analytics)
* Storage accounts need to:
    * Have a unique name (unique to **everyone**)
    * Unique name must be lowercase or numbers
    * Blob storage is accessible using [https://storage_name.blob.core.windows.net](https://storage_name.blob.core.windows.net) 
    * File storage is accessible using [https://storage_name.file.core.windows.net](https://storage_name.blob.core.windows.net) 

Azure Blobs (binary large objects)



* The most popular form of cloud object storage
* Some features of blob storage
    * Can store massive files
    * Can store any file type
    * Data is unstructured 
    * Blobs are stored in containers
        * Each storage account have have many containers
        * Each container has its own unique web address
        * [https://storage_acount.blob.core.windows.net/container_name/blob](https://storage_acount.blob.core.windows.net/container_name/blob)
        * Each container can have folders to store blobs in
* Blob types
    * Block
        * Stores text or binary data
        * 4TB limit
        * The default blob type
    * Append
        * A block blob that is optimised for data that is consistently added such as an update log
    * Page
        * Mainly designed such that any part of a file can be accessed at any time
        * 8TB limit
        * Normally used as virtual hard drives for VMs
* Use case of blob storage
    * Media repository for a website / streaming service
    * File storage (though better served using a file server)
    * Archiving dataS
    * Data for analytics
* Blob storage tier (cheaper cost for infrequent or slower data retrieval)
    * Hot			Frequent access
    * Cool			Occasional access
    * Cold			Infrequent access
    * Archive		Almost never accessed
    * Non-hot storage options have a minimum retention period; this is a minimum time period which the piece of data will stay in blob storage before it can be deleted; this means keeping files in non-hot storage for less than the minimum retention period will incur an additional cost
* Blob storage tiers can be:
    * Set either hot or cool by default on an storage account level
    * We can set individual blobs to be set to hot, cool, cold or archive 
        * This process happens when you upload a file using Azure portal, it will give you the option to select the access tier
        * We can also change an already stored blob to a different tier
* Blobs by default will have public access denied
    * In order to allow public access, we need to enable blob anonymous access in the storage account as well as enable blob anonymous access on the appropriate containers (this will set the anonymous access level to all items in the container)

<table>
  <tr>
   <td>
   </td>
   <td>
Storage cost
   </td>
   <td>Access cost
   </td>
   <td>Retrieval time
   </td>
   <td>Minimum retention
   </td>
   <td>Examples
   </td>
  </tr>
  <tr>
   <td>Hot
   </td>
   <td>High
   </td>
   <td>None
   </td>
   <td>Instant
   </td>
   <td>None
   </td>
   <td>Streaming
   </td>
  </tr>
  <tr>
   <td>Cool
   </td>
   <td>Low
   </td>
   <td>Yes
   </td>
   <td>Instant
   </td>
   <td>A month
   </td>
   <td>Backup
   </td>
  </tr>
  <tr>
   <td>Cold
   </td>
   <td>Very Low
   </td>
   <td>Yes
   </td>
   <td>Instant
   </td>
   <td>Quarter of a year
   </td>
   <td>Seasonal data
   </td>
  </tr>
  <tr>
   <td>Archive
   </td>
   <td>Lowest
   </td>
   <td>Yes
   </td>
   <td>Slow (hours)
   </td>
   <td>Half a year
   </td>
   <td>Compliance
   </td>
  </tr>
</table>


Azure disk [storage]



* Disks are storage entities for VMs
    * Both disk and VM must be in the same region
    * Utilises block storage (page blob storage)
    * Is provided as a managed service; its unmanaged service is being retired
    * Disks can import .vhd files from on-premise virtual machines and use these disks on Azure VMs 
* Disks are not tied to a storage account and therefore there is no 'management' of disk storage unlike blob storage

<table>
  <tr>
   <td>
   </td>
   <td>
HDD
   </td>
   <td>Standard SSD
   </td>
   <td>Premium SSD
   </td>
   <td>Premium SSD v2
   </td>
   <td>Ultra disk
   </td>
  </tr>
  <tr>
   <td>Type
   </td>
   <td>Mechanical
   </td>
   <td>Solid state
   </td>
   <td>Solid state
   </td>
   <td>Solid state
   </td>
   <td>Solid State
   </td>
  </tr>
  <tr>
   <td>Cost
   </td>
   <td>Low 
   </td>
   <td>Okay
   </td>
   <td>High
   </td>
   <td>Very high
   </td>
   <td>Ultra high
   </td>
  </tr>
  <tr>
   <td>Speed
   </td>
   <td>Slow
   </td>
   <td>Fast
   </td>
   <td>Very fast
   </td>
   <td>Super fast
   </td>
   <td>Ultra fast
   </td>
  </tr>
  <tr>
   <td>Uses
   </td>
   <td>Backups
   </td>
   <td>General \
Web server
   </td>
   <td>Analytics \
Business
   </td>
   <td>Analytics \
Business
   </td>
   <td>Database
   </td>
  </tr>
  <tr>
   <td>OS installable
   </td>
   <td>Yes
   </td>
   <td>Yes
   </td>
   <td>Yes
   </td>
   <td>No
   </td>
   <td>No
   </td>
  </tr>
  <tr>
   <td>Capacity
   </td>
   <td>32TB
   </td>
   <td>32TB
   </td>
   <td>32TB
   </td>
   <td>64TB
   </td>
   <td>64TB
   </td>
  </tr>
</table>


Azure Files



* A file share server
    * Supports SMB (Windows) and NFS protocols (Linux)
    * Available on all major operating systems
    * Can replace on-premise file servers or sync to an on-premise file server using Azure File Sync
    * Using a file server allows compatibility with most applications and powershell scriptlets and 
* The use case of Azure Files
    * Automate backups
    * Infinite storage capacity
    * Enforce security 
        * Integrates with on-premise active directory or Azure Active Directory Domain Service (AADDS)
    * Easy to share files 

Premium storage



* Premium storage has better performance than the standard general-purpose v2 storage but has a few trade offs:
    * Only local redundancy / zone redundant storage (no multi-region storage redundancy)
    * Not compatible with all storage types
    * Expensive
* Premium block blobs
    * Provides high transaction speeds / low latency storage
    * Useful for IoT and AI applications
    * Only supports block blob storage
* Premium page blobs
    * Provides API access
    * Good for enterprise solutions that need scalability
    * Also the storage type used for VMs
* Premium file share

Azure Tables



* A noSQL database for structured data
* Can store non-relational (not rows and columns) data such as key-value sets
* Integrates with hybrid and multi-cloud setups
* Lightweight and cost-effective way to store noSQL data opposed to more advanced options such as Azure SQL or Cosmos DB
* Somewhat superseded by Cosmos DB

Azure Queues



* A message storage service for asynchronous task processing
* Some examples of asynchronous task processing includes:
    * Tickets
    * Email
    * Messaging apps
    * Event notifications
    * Order processing (like ordering items from an e-commerce website) 
    * Internet of Things

Azure Data Lake



* Azure Data Lake is a service that stores large amounts of data and analyses them
* The main use of Azure Data Lake is for data analytics and machine learning
* Some features of Azure Data Lake over other storage services
    * It can handle huge amounts of data (petabytes)
    * It can perform analyses and data transformation using programming languages such as .NET and Python
    * It comes with all the default features of Azure such as security and scalability and ability to handle data in all different forms

Methods of data redundancy



* Causes of data loss
    * Hardware failure
    * Server outage
* Azure provides redundancy by always creating an automatic copy of data (minimum 3 copies)
* Redundancy options in Azure
    * Single zone
        * Locally-redundant storage (LRS)
            * Cheapest option
            * Data is replicated within a data centre
            * Copies are kept on different disks but same data centre and same region / availability zone so it does not protect against zone or regional outage
        * Zone-redundant storage (ZRS)
            * Data is stored in different availability zone
            * Data is stored in the same region
    * Multiple regions
        * Geo-redundant storage (GRS)
            * Data is stored in a primary zone and a secondary zone in **different regions**
            * Data within a zone may be kept in the same data centre (but not same disk)
            * Comes with the option of making read access of secondary zone automatic in the event of a primary zone outage (not a default option)
        * Geo-zone-redundant storage (GZRS)
            * Data is stored in a primary zone and a secondary zone in different regions
            * Data is stored in different availability zones within a primary zone whereas data in the secondary zone will be kept in the same availability zone 
            * Comes with the option of making read access of secondary zone automatic in the event of a primary zone outage (not a default option)
    * 3 copies of the data will be stored in any primary region
    * 3 copies of the data will be stored in any secondary region (multi-region redundancy only)

Methods of data transfer



* AzCopy
    * A command line utility (downloadable executable) that can transfer blobs and files from Azure
    * Usually used with powershell or bash scripts to automate file transfer
    * Mainly used for occasional file transfers
    * azcopy cp **"filename" "[https://storage_account.blob.core.windows.net/container](https://storage_account.blob.core.windows.net/container)"** will copy a filename to the storage_account container named "container"
* Azure Storage Explorer
    * A windows explorer look-a-like that can move files (blob or non-blob) to and from Azure 
    * Graphical interface makes it more user-friendly
* Azure File Sync
    * Synchronises files between an on-premise file server and the Azure Files 
    * Mainly used for:
        * Back up
        * Remote users
        * Transition from on-premise file server to cloud-only file server usage
        * Synchronise files between multiple on-premise file servers
* Azure Data Box
    * A physical hard drive (box) is shipped to an address
    * Users can then upload data to the hard drive to upload to Azure or download data from the hard drive that has been preloaded with contents from Azure
    * This option is mainly used for:
        * Massive data transfer (like terabytes)
        * Disaster (backup) recovery
        * Security requirements (data cannot be transferred over internet)
* Azure Migrate
    * Migrate is a tool that helps moves on-premise servers, databases and applications onto Azure
    * It can discover resources that need to be migrated
    * It can migrate VMs
    * It can migrate databases
    * It can migrate on-premise applications and its dependencies
    * It can migrate using Azure Data Box
