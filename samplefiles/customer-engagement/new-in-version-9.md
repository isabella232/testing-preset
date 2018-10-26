---
title: "What's new in Customer Engagement for Dynamics 365 (online)| MicrosoftDocs"
description: ""
keywords: ""
ms.date: 09/20/2018
ms.service:
  - "dynamics-365-crossapp"
ms.custom:
  - "dyn365-hub"
ms.topic: article
applies_to:
  - "Dynamics 365 (online)"
  - "Dynamics 365 9.x"
ms.assetid: 994cc854-17f6-45d6-bc20-fcf1a3f2dad6
author: shellyhaverkamp
ms.author: shellyha
manager: annbe
---

# What's new in Dynamics 365 (online), version 9 (Customer Engagement) 

[!INCLUDE [cc-whats-new-spring-18-release-notes](../../../includes/cc-whats-new-spring-18-release-notes.md)]

# What's new in version 9
If you're a new customer, [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)] is available for [trial](https://trials.dynamics.com/) or [purchase](https://www.microsoft.com/dynamics365/pricing). If you're an existing customer, learn how to [manage updates](https://docs.microsoft.com/dynamics365/customer-engagement/admin/manage-updates). 

See also these links:

- Learn about late-breaking issues in the [Readme](https://docs.microsoft.com/dynamics365/customer-engagement/admin/readme-9).

- Learn about what's new in [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)] [for developers](new-in-version-9-for-developers.md). 

## Areas of investment
The main areas of investment in the version 9 release are:

-   **UX enhancements** to improve readability and usability of the web apps,
    and to make data entry faster and easier.

-   **Extensibility and app platform enhancements**, including improvements to
    security and data management.

Additionally, there are **enhancements to the in-app Designer tools** that allow admins and customizers to tailor apps through a graphical user interface instead of writing code (App Designer, Site Map Designer, and Business Process Flow Designer).

- A new **Unified Interface** framework used for the Customer Service Hub,
  [!INCLUDE [pn-dyn-365-phones](../../../includes/pn-dyn-365-phones.md)] and [!INCLUDE [pn-dyn-365-tablets](../../../includes/pn-dyn-365-tablets.md)], and [!INCLUDE [pn-crm-app-for-outlook-short](../../../includes/pn-crm-app-for-outlook-short.md)].
  Unified Interface is also available in the App Designer so that customizers
  can build app modules using this new look and feel.
    
## User experience enhancements in web apps 

With this release, the user interface of the web apps has been refreshed to
improve usability and visual appeal. These changes are consistent across these
web apps: Sales, Customer Service, Field Service, and Project Service
Automation. The changes apply to all the main application areas such as forms,
dashboards, grids, dialogs, and the search screen.

## User interface refresh (applies to all web apps)

Now users will see forms with customer data grouped in easy-to-read containers
that streamline data entry. There’s new field styling to make empty fields
easier to see, and the text wraps within fields to improve readability.

The user interface changes include:

-   **Removal of unneeded whitespace** on forms and dashboards. Containers for
    content now have defined borders. There is consistent spacing between
    sections. Empty containers have a helpful message and icon.

    ![Example of improved interface](media/user-interface-refresh.png "Example of improved interface")

-   **Improved visual hierarchy** by means of a new clipboard structure for the
    content shown on all pages, such as forms, dashboards, and grids. The page
    and panel header colors used for the clipboard are customizable.

-   **Use of standardized fonts** for a more consistent look and feel.

-   **More intuitive user experience** for elements such as tabs, buttons, and
    input fields on forms to help users be more productive.

## Top customer asks

These enhancements address popular feature requests from customers:

-   **On forms, long text labels and values are wrapped.** Admins can control
    word wrap through system level settings.

-   **The color of a sub-grid header can be customized at the form level.**

To change the color:

1.  Go to **Settings** \> **Customizations** \> **Customize the System** and
    select the form for an entity you want to change.

2.  Open a record, double-click on a subgrid, and enter the color choice in the
    header field. Use only the hex color schemes. For example, the code \#fofofo
    represents grey.

-   **There are now three new standard themes to choose from:**

    -   CRM Blue Theme

    -   CRM Default Theme

    -   CRM Orange Theme

To customize a theme:

-   Go to **Settings** \> **Customizations** \> **Themes** and clone the theme
    you want to customize. Selecting a header color in a theme will
    auto-populate the rest of the theme colors with system-suggested defaults
    that can be edited.
    
### Advanced find 

Advanced find now has the option to build a **NOT IN** query. For example, users
can query for all cases that do not have a related task.

To do this, users launch advanced find from the icon on the navigation bar. In
the query, they choose what type of record to look for, and then select a
related record type to see the **Does not contain data** operator.

More information: [Use advanced find](https://docs.microsoft.com/dynamics365/customer-engagement/basics/save-advanced-find-search)

## Unified Interface framework for new apps

In this release, we’ve invested in a new Unified Interface framework that
provides a uniform experience for all new applications. We designed the Unified
Interface framework from the ground up with accessibility in mind, which means:

-   People with screen readers can skip to content directly and navigate to
    sections that are important to them.

-   People using reading plugins receive great results.

-   People using browser plugins can jump to specific sections on a page.

-   Keyboard users can save time and effort by using the tab key and keyboard
    shortcuts.

The Unified Interface also uses responsive web design principles to provide an
optimal viewing and interaction experience for any screen size, device, or
orientation. For example, subgrids morph into lists for smaller screen sizes.

## Public Preview: Dynamics 365 Channel Integration Framework

Using the Channel Integration Framework Administrator App, you can configure channel providers for your Dynamics 365 organization. You can configure channels like voice, chat, SMS, social media, and any channel that has JavaScript-based widgets and adheres to the standard JavaScript APIs exposed by the Channel Integration Framework library.

More information: [Channel Integration Framework](/dynamics365/customer-engagement/developer/channel-integration-framework/channel-integration-framework)

## Introducing: Dynamics 365 for Marketing (now generally available)

[!INCLUDE [pn-dyn-365-marketing](../../../includes/pn-dyn-365-marketing.md)] is a marketing-automation application that helps turn prospects into business relationships. The app is easy to use, works seamlessly with [!INCLUDE [pn-dyn-365-sales](../../../includes/pn-dyn-365-sales.md)], and has built-in business intelligence. 

More information: [Overview](/dynamics365/customer-engagement/marketing/overview)

### Create graphical email messages and online content to support marketing initiatives

Customizable templates for emails and landing pages help amplify your digital voice. Intuitive drag-and-drop design tools simplify content creation—from personalizing the message to setting up lead scoring.

![Marketing designer](media/marketing-designer-pages.png "Marketing designer")

More information: [Design your digital content](/dynamics365/customer-engagement/marketing/design-digital-content)

### Design interactive customer journeys to nurture leads with personalized experiences

Use the drag-and-drop journey designer to create an automated, multichannel campaign that sends personalized email messages, generates follow-up activities, launches workflows, and more. Each contact in the target group travels down a customized path that reacts to their interactions and identifies your best prospects. Easily track campaigns and analyze results to build profitable long-term relationships.

![Customer journey designer](media/marketing-customer-journey.png "Customer journey designer")

More information: [Customer journey designer](/dynamics365/customer-engagement/marketing/customer-journeys-create-automated-campaigns)

### Organize and publicize events

Keep all the information about your event venues, logistics, ticketing, sessions, speakers, sponsors, and more in one place so your whole team can coordinate while working on them. Then generate an online event portal where attendees can review event information and register online. Integrate your events into your marketing email messages and customer journeys to help get the word out.

![Event portal](media/marketing-event-portal.png "Event portal")

More information: [Event planning and management](/dynamics365/customer-engagement/marketing/event-management)

### Prioritize leads for more wins

Set up automated lead-scoring rules that automatically identify your hottest leads based on how they interact with your events and customer journeys. As soon as a lead meets an agreed-on sales-ready score, the system automatically routes it to a salesperson to follow up while the lead's still hot.

![Lead score model](media/marketing-designer-lead-score-model.png "Lead score model")

More information: [Score and manage leads](/dynamics365/customer-engagement/marketing/score-manage-leads)

### Make survey results more actionable
Easy-to-create surveys make it simple to gather actionable feedback from customers. Understand individual customer needs and expectations so you can grow relationships and revenue.

### Share information across teams
Securely share information about leads and contacts across your business and understand how every interaction affects your results. Connect sales and marketing processes to automate follow-ups and track the progress of every lead.

### Analyze and document your marketing return on investment (MROI)
Use dashboards and reports to track the performance of your marketing initiatives, and to identify your best lead sources and marketing activities. Bring together sales and marketing results to track and increase their impact on your business.

### Tap into LinkedIn's business prospects
Quickly target and connect with the right LinkedIn audiences by importing leads generated with LinkedIn's lead tools directly into Dynamics 365.

More information: [Integrate with LinkedIn Lead Gen](/dynamics365/customer-engagement/marketing/linkedin-lead-gen-integration)

#### Configure and expand the application
Customize the application to fit your specific business needs. Make basic customizations by using tools built right into the app. Expand its capabilities and add new features by installing third-party packages from our thriving marketplace—Microsoft AppSource. And it's easy to connect with Dynamics 365 partners to get expert help. The Marketing app is built on the same platform and database as the sales app, so both teams share the same records, and customizers can leverage their existing knowledge when adding custom features.

## New [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] Connector solution

A new solution, initially available for version 8.2 of [!INCLUDE [pn-crm-online](../../../includes/pn-crm-online.md)], allows
users to run [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] lead generation ad campaigns, and then sync resulting
leads with [!INCLUDE [pn-dyn-365-sales](../../../includes/pn-dyn-365-sales.md)]. It will be updated for version 9.0 soon after
the initial release. The new solution will be available on AppSource and is called
Microsoft [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] Connector for [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] Lead Gen
Forms.

The solution includes:

- **Support for multiple [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] member accounts.** Set up your [!INCLUDE [pn-crm-online](../../../includes/pn-crm-online.md)]
  organization to access and bring in leads from campaigns run by multiple
  employees using different [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] member profiles.

- **Customizable lead-matching strategies.** Customize lead-matching
  strategies to define which fields the system uses to find matches with
  [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] leads. For example, you can match on someone’s email address,
  last name, company name, or other field. When there’s a match, the data from
  the person’s [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] profile is included in corresponding fields on the
  lead form.

- **Ability to analyze lead performance across sources.** Track and analyze
  the performance of leads captured on [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] and compare them against other
  sources.

To use the [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] Connector with [!INCLUDE [pn-crm-online](../../../includes/pn-crm-online.md)], you’ll need access to the
[!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] Campaign Manager as part of your [!INCLUDE [pn-linkedin](../../../includes/pn-linkedin.md)] subscription. You’ll also
need to use [LinkedIn’s Lead Gen
Forms](https://business.linkedin.com/marketing-solutions/native-advertising/lead-gen-ads)
to run native ads.

More information: [LinkedIn connector](https://docs.microsoft.com/dynamics365/customer-engagement/linkedin/sync-linkedin-leads)

## Customer Service Hub

With this release, the Customer Service Hub (called Interactive Service Hub in
earlier releases) has been rebuilt on the new Unified Interface as a stand-alone
application.

The Customer Service Hub shows you all your vital customer service information
in one place, and makes it easier for reps and managers to prioritize and act on
service cases.

> [!NOTE]
> If you're a developer, see also [What's new for developers](https://docs.microsoft.com/dynamics365/get-started/whats-new/customer-engagement/new-in-version-9-for-developers).

### Dashboards and charts

You can access all the system and user dashboards from within your Unified Interface apps. The interactive dashboards are now available for all record types with richer interactive dashboard capabilities. 

![Unified Interface dashboard](media/uci-interactive-dashboard.png "Unified Interface dashboard")

### Reference panel 

Use the reference panel for apps built on Unified Interface like Dynamics 365 for Customer Service. The reference panel is a great way to get work done without clicking away from the screen you are on. You can look up other things like knowledge base articles within the context of the record you are viewing. 

### New and improved business process flows 

The stages in a business process flow can now be displayed in floating mode,
along with docked mode. Stages can now be aligned in a vertical layout, instead
of horizontal, which makes it easier to see which steps are required to be
completed before moving forward. You can also choose to include an optional step
in the business process flow and define criteria to trigger it. Business Process
flow is now an entity and you can create custom views. Business Process entities
can now be made available on the site map.

### Timeline and activity feed enhancements

An improved timeline lets service reps view all customer interactions for a case
in a single stream. Reps can create, update, and manage notes, posts, and other
interactions directly on the timeline. The Activity feed on the timeline gives
the service team visibility into what’s going on so they can resolve cases and
collaborate more effectively.

The timeline includes textual and visual filters that let reps view and sort
activity types to help them focus on the just the details they need. Reps can
keep track of what they may have missed from the previous day or week in the
What’s new section, which shows new notes, unread emails, and new activities
created while they were away.

### Activity management

New Quick Create forms have been introduced for Task, Phone Call, and
Appointment with customization capabilities. You can also benefit from the
updated email editor control with its rich editing capability.

### Knowledge Management 

With the latest release, Knowledge Management is based on the new Unified
Interface, and is included as a part of Customer Service Hub. You can author,
edit, search, publish, and translate the knowledge articles using Knowledge
Management.

Some of the key enhancements are:

- **Advanced options to create content in the rich-text editor.** You can now
  preview the content to view its compatibility on multiple devices, like
  tablets or phones.

- **Better support for editing the HTML source** of the knowledge article.

More information: [Customer Service Hub overview](https://docs.microsoft.com/dynamics365/customer-engagement/customer-service/overview)

## Outlook app

The updated version of [!INCLUDE [pn-crm-app-for-outlook-short](../../../includes/pn-crm-app-for-outlook-short.md)] is now available as a preview feature for [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)].

With [!INCLUDE [pn-crm-app-for-outlook-short](../../../includes/pn-crm-app-for-outlook-short.md)], users can tap the power of [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] while using [!INCLUDE [pn-ms-outlook-short](../../../includes/pn-ms-outlook-short.md)]—a
tool they’re already familiar with. 

The new version of [!INCLUDE [pn-crm-app-for-outlook-short](../../../includes/pn-crm-app-for-outlook-short.md)] is built on the Unified Interface framework. The app keeps the functionality from the previous version, but adds additional capabilities that come with the Unified interface. 

### View list items

See list items for any view or grid that's accessible through the app.

![Outlook app list items example](media/outlook-app-view-list-items.png "Outlook app list items example")

### Site map

Take advantage of the [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] sitemap to easily access 
favorite and recently used records in [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)].

![Outlook app sitemap](media/outlook-app-sitemap.png "Outlook app sitemap")

### Detailed record view

Navigate to records within the app and edit them.

![Outlook add detailed records](media/outlook-app-detailed-records.png "Outlook app detailed records")

### Relevance search

Use the global search UI to search, view, and access [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)]
records.

![Relevance Search from Outlook app](media/outlook-app-relevance-search.png "Relevance Search from Outlook app")

More information: [Dynamics 365 App for Outlook overview](https://docs.microsoft.com/dynamics365/customer-engagement/outlook-app/overview)

## Dynamics 365 mobile app

The new mobile app is built on the new Unified Interface, which provides key
accessibility and responsive design benefits. Current users will not need to
download an update from the app store. They will receive the new functionality
when the [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] server is updated to the latest version.

### New navigation

The new navigation on mobile lets you quickly navigate to the different areas in
the system – Sales, Service, Marketing, and more. It also provides quick access
to recently-viewed records and pinned favorites.

![New mobile navigation](media/navigation-mobile-sales.png "New mobile navigation")

### Take action on record

You can now take action on a record without opening the record. From a list of
records, tap the **More** button (…), and then select an action such as
**Delete**, **Reassign**, or **Close**. You can take the same action when you
select multiple records.

### iFrame and web resource support in [!INCLUDE [pn-dyn-365-phones](../../../includes/pn-dyn-365-phones.md)]
If you can add iFrames and web resources in forms and dashboards in a [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] web app, they will be enabled in [!INCLUDE [pn-dyn-365-phones](../../../includes/pn-dyn-365-phones.md)] as well if you
check the box to enable iFrames and web resources for phones. For example, if
you add a news feed to a dashboard in a web app, the news feed will also appear
in the phone app.

<!--### Continuum support for Windows Phone

Use your phone like a PC with Continuum support. You can connect a Windows Phone
mobile device to a larger screen, allowing you to utilize your phone as a PC.
Use a dock or adapter to connect to a monitor, keyboard, and mouse, and then use
the mobile app on your Windows 10 phone and see your content on a larger screen.
When your phone is connected to another screen, the mobile app reflows to fit
the larger screen size. You can also continue to use your phone the way you
normally would without interrupting what’s playing on the larger screen. This
offers a natural, no compromise, and familiar method to seamlessly switch
between a smaller device to a bigger device, without impacting your
productivity. [Learn more about
Continuum](https://www.microsoft.com/windows/Continuum).-->

<!--### Mobile offline

With the new Unified Interface, you can get offline faster. When you go offline,
you don’t have to wait for all the data to download. Once the prerequisite
entity data download is complete, you can start working while the system
continues to download data. You can also track the status of the download and
see how long it will take, including detailed status for each entity.
-->

More information: [Dynamics 365 for phones and tablets User Guide](https://docs.microsoft.com/dynamics365/customer-engagement/mobile-app/dynamics-365-phones-tablets-users-guide)

## Extensibility and app platform 

New capabilities added to the in-app visual tools allow business users to easily
tailor apps through a graphical user interface, without writing code.

The App Designer has UX improvements to simplify the way admins and customizers
create their own solutions. There are also updates to the My Apps landing page
and the Sitemap Designer.

> [!NOTE]
> If you're a developer, see also [What's new for developers](https://docs.microsoft.com/dynamics365/get-started/whats-new/customer-engagement/new-in-version-9-for-developers).

### App Designer

App Designer includes the following new features:

-   Optionally, choose an existing solution and/or sitemap to quickly create
    your app.

-   Choose the client type—web or Unified Interface (to take advantage of
    built-in accessibility and responsive design improvements). For more
    information on the new Unified Interface, see [Unified Interface framework
    for new apps](#unified-interface-framework-for-new-apps) earlier in this
    guide.

-   Support for interactive dashboards with apps created for clients based on
    the Unified Interface framework.

-   Find components easily from the App Designer canvas. Click **Search
    Canvas**, and then enter a keyword for the component you’re looking for in
    the search box. The search pane organizes the results. Click a result to
    highlight the search item throughout the App Designer canvas.

    >![App Designer screen](media/app-designer-canvas.png "App Designer screen")

-   If needed, enable your app to support mobile offline by selecting one or
    more mobile offline profiles.

-   Add an optional custom welcome page from a web resource, which becomes the
    first page to load when the app is opened. Welcome pages can provide
    guidance and other key information to users upon app startup.
    
More information: [App Designer overview](https://docs.microsoft.com/dynamics365/customer-engagement/customize/design-custom-business-apps-using-app-designer)

### Site map Designer

Site map Designer includes the following new features:

-   Set an interactive dashboard as the default dashboard subarea in the sitemap
    for apps based on the Unified Interface framework.

-   Cut, copy, and paste sitemap components.

-   Support for miscellaneous security privileges within app subareas.

    ![Site map Designer miscellaneous privileges](media/sitemap-designer-miscellaneous-privileges.png "Site map Designer miscellaneous privileges")

-   Inline editing support for sitemap components. To edit inline, hover over
    the component to reveal the pencil.

    ![Site map Designer showing inline editing](media/sitemap-designer-inline-editing.png "Site map Designer showing inline editing")
    
More information: [Create a site map](https://docs.microsoft.com/dynamics365/customer-engagement/customize/create-site-map-app)

### View Designer

Use the new WYSIWYG View Designer together with the App Designer. The View Designer provides these features:

- Intuitive drag-and-drop experience for adding and rearranging fields 
    
- Search fields in the Field explorer 
    
- Sort columns with a single click in the column header 
    
- Single-click access to column properties 
    
- Side-by-side configuration of filters and columns for better configuration experience
    
- Sample data in grids to provide a near runtime snapshot of the view 
    
  ![View Designer](media/view-designer.png "View Designer")

### Ability to filter and search on My Apps landing page

The My Apps landing page enhancements include an improved user interface that
has app filtering and app search capabilities. Responsive design makes the My
Apps page better suited for small screens.

### Interact with data from external systems using new “virtual” entities

A virtual entity is a custom entity in [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] that retrieves data at
runtime from an external data source. Virtual entities appear in [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] to
users as regular [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] entity records, but contain data that is sourced
from an external database, such as an [!INCLUDE [pn-azure-shortest](../../../includes/pn-azure-shortest.md)] SQL Database. An OData v4 data
provider is included so you can connect to data sources without the need to
develop your own OData v4 data provider.

Records based on virtual entities are available from all [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] clients,
including custom applications developed using the [!INCLUDE [pn-sdk](../../../includes/pn-sdk.md)].

Virtual entities provide these benefits:

- **End users** work with the records created by the virtual entity to view
  the data in fields, grids, search results, and Fetch XML-based reports and
  dashboards.

- **System customizers** can configure the data source record and create
  virtual entities without writing any code.

- **Developers** can implement plugins to read external data using the
  [!INCLUDE [pn-sdk](../../../includes/pn-sdk.md)] and [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] Plug-in Registration tool.

  ![Virtual entity dialog box](media/virtual-entity-create.png "Virtual entity dialog box")

Create a virtual entity like any custom entity, and then select the **Virtual
Entity** check box.

Selecting the check box displays additional information requirements for the data source, as well as the External Name and External Collection Name values for the entity definition.

> [!NOTE]
> If you're a developer, see also [What's new for developers](https://docs.microsoft.com/dynamics365/get-started/whats-new/customer-engagement/new-in-version-9-for-developers).

More information: [Create a virtual entity](https://docs.microsoft.com/dynamics365/customer-engagement/customize/create-edit-virtual-entities)

### Multi-step workflow automation with embedded Microsoft Flow 

[!INCLUDE [pn-flow](../../../includes/pn-flow.md)] is a cloud-based service that makes it practical and simple for
business users to build workflows that automate time-consuming business tasks
and processes across applications and services.

This release includes the ability to run Microsoft Flows from within [!INCLUDE [pn-crm-online](../../../includes/pn-crm-online.md)], making it simple for users to combine a broad spectrum of services that can
be initiated from within [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] without writing code. 

More information: [Microsoft Flow](https://ms.flow.microsoft.com/documentation/connection-dynamics365/)

### Power BI enhancements
You can now embed [!INCLUDE [pn-power-bi](../../../includes/pn-power-bi.md)] dashboards and tiles in [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] selected from
group-based [!INCLUDE [pn-power-bi](../../../includes/pn-power-bi.md)] App Workspaces. Previously, dashboards and tiles could only
be embedded from My Workspace.

![Power BI dialog with group-based workspaces](media/power-BI-group-based-workspaces.png "Power BI dialog with group-based workspaces")

More information: [Power BI](https://docs.microsoft.com/dynamics365/customer-engagement/analytics/customize-power-bi-content-packs)

### Business process flow enhancements

We made the following enhancements to business process flows:

-   **Business process flow as Action steps**  
    Action steps allow the execution of server-side business logic by calling
    on-demand Process Actions. You can now include an optional step in a process
    and define criteria to trigger it. For example, you can create a Process
    Action that automates sending an email, creating a task, or manipulating
    data. This Process Action can be called by the user with a click of a button
    that shows as one of the steps in the stage they are working on.

-   **Business process flows in sitemap, views, and grids**  
    Business Process entities can now be displayed on the sitemap. This makes it
    easier for people to work with process first as opposed to data first, which
    is less natural. Business Process entities can be included in views, charts,
    and dashboards, which brings the process data to the forefront of the
    application.

-   **Business process flow as an entity now supported in Interactive Experience
    Dashboard**  
    Because a business process flow is now an entity and you can create custom
    views, it’s possible to leverage the Interactive Experience Dashboards to show processes 
    as streams and queues so that users can be more productive
    and know which process to act on next.

> [!NOTE]
> If you're a developer, see also [What's new for developers](https://docs.microsoft.com/dynamics365/get-started/whats-new/customer-engagement/new-in-version-9-for-developers).

Charts can display multiple angles of the process, such as:

-   Process funnel (active process count by stage)

-   Process count by elapsed time (which processes are getting old and should be
    acted on quickly)
-   Process count by status (how many processes are inflight vs abandoned vs
    finished)

-   Process velocity (how many processes closed each month)

More information: [Business process flows overview](https://docs.microsoft.com/dynamics365/customer-engagement/customize/business-process-flows-overview)

### MultiSelect option set
Customizers can now add multi-select fields to forms, quick view and quick
create forms, and read-only and editable grids. When you add a MultiSelect
Option Set field, you can specify multiple values for the field that users can
select, up to 150. For example, include multiple locations or countries in an
**Area of operation** field. A user can select one, more than one, or all
locations from the list of available values.

![Multiselect option set example](media/multiselect-option-set.png "Multiselect option set example")

> [!NOTE]
> If you're a developer, see also [What's new for developers](https://docs.microsoft.com/dynamics365/get-started/whats-new/customer-engagement/new-in-version-9-for-developers).

### Web resource dependencies and localization

This release of [!INCLUDE [pn-dyn-365-online](../../../includes/pn-dyn-365-online.md)] includes improvements in how web resources are
managed and localized.

#### Web resource dependencies

In previous releases, web resources, including script dependencies, strings,
script libraries, and so on, were managed in an ad-hoc manner. In this release,
you can now specify web resources during customization that will be used at
run-time to include dependencies. This makes it easier to ensure that HTML,
[!INCLUDE [pn-javascript](../../../includes/pn-javascript.md)] resources, and all dependent resources are loaded appropriately.

#### Web resource localization

This release also introduces simplified localization of resource strings.
Currently there is no easy way for solution developers to use localized strings
in their [!INCLUDE [pn-javascript](../../../includes/pn-javascript.md)] web resources. Most developers use a JSON based hard-coded
approach like [the one documented here](https://msdn.microsoft.com/library/hh670609.aspx#BKMK_DeveloperOption)
which is neither efficient nor scalable. This release enables the localization
of strings used in web resources as a first-class component for solutions. This
will make it easy for apps/solutions to be available in multiple languages and
improve the process for app teams to localize their solutions.

This release also includes support for a new resource type, RESX, which is an
XML-based file format that supports comments associated with key+value
translation pairs and is supported in [!INCLUDE [pn-visual-studio-short](../../../includes/pn-visual-studio-short.md)]. For more information about
RESX, see [Resources in .Resx file formats](https://msdn.microsoft.com/library/ekyft91f(v=vs.80).aspx).

![Solution Explorer dialog box](media/solution-explorer.png "Solution Explorer dialog box")

> [!NOTE]
> If you're a developer, see also [What's new for developers](https://docs.microsoft.com/dynamics365/get-started/whats-new/customer-engagement/new-in-version-9-for-developers).


### Command bar theming

Now you can customize a command, choose different colors, and change the color
of the text to black or white.

## See also

[What's new in Unified Service Desk](/dynamics365/customer-engagement/unified-service-desk/admin/whats-new-unified-service-desk-administrators)
