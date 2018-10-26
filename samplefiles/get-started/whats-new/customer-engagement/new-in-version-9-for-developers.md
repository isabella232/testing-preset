---
title: "What's new for developers in Dynamics 365 (online) Customer Engagement| MicrosoftDocs"
ms.date: "03/21/2018"
ms.topic: "article"
applies_to: 
 - "Dynamics 365 (online)"
 - "Dynamics 365 9.x"
ms.assetid: "994cc854-17f6-45d6-bc20-fcf173f2d6d6"
searchScope:
  - "Dynamics 365"
  - "Developers"
  - "Customer Engagement"
ms.custom:
 - dyn365-hub
ms.service: dynamics-365-crossapp
author: kumarvivek
ms.author: kvivek
manager: annbe
---

# What's new for developers in Dynamics 365 (online), version 9

[!INCLUDE [cc-whats-new-spring-18-release-notes](../../../includes/cc-whats-new-spring-18-release-notes.md)]

We're excited to announce that [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)] is available for [trial](https://trials.dynamics.com/) and [purchase](https://www.microsoft.com/dynamics365/pricing)! Stay tuned for information about when you can update your existing organizations.

See also these links:

- Learn about late-breaking issues in the [Readme](https://docs.microsoft.com/dynamics365/customer-engagement/admin/readme-9).

- Learn about what's new in [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)] [for admins and end users](new-in-version-9.md).  

[!INCLUDE [cc-custeng-definition](../../../includes/cc-custeng-definition.md)]

## Pubic Preview: Dynamics 365 Channel Integration Framework

Channel Integration Framework is a set of JavaScript APIs (methods, events, and protocols) that enable developers and partners to build immersive communication experiences so that third-party communication widgets running on channel provider clouds can interact with Dynamics 365.

With the Channel Integration Framework application (solution), you can configure the channel in the Unified Interface app so that your agents can access it to serve your customers. 

More information: [Channel Integration Framework](/dynamics365/customer-engagement/developer/channel-integration-framework/channel-integration-framework) 

## API limits

Beginning March 19, 2018 we will limit the number of API requests made by each user within five minutes. When this limit is exceeded, an exception will be thrown by the platform.

The limit will help ensure that users running applications that make extraordinarily large demands on servers will not affect other users. The limit will not affect normal users of the platform. Only applications that perform a very large number of API requests will be affected. Based on telemetry data analysis, this limit is well within the bounds of most applications that perform a large number of API requests. The limit will help provide a level of protection from random and unexpected surges in request volumes that threaten the availability and performance characteristics of the [!INCLUDE [pn-dyn-365](../../../includes/pn-dyn-365.md)] platform.

More  information: [API Limits](/dynamics365/customer-engagement/developer/api-limits)


## Security updates may require update to custom client applications
Starting with [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)] we will begin requiring connections to customer engagement applications to utilize TLS 1.2 (or better) security. This aligns with updated Microsoft and industry security policies and best practices, and you may be required to take actions to maintain connectivity to [!INCLUDE [pn-dyn-365](../../../includes/pn-dyn-365.md)] customer engagement applications.

The most common fix for custom client applications built utilizing .NET Framework 4.5.2 is that they will need to be re-compiled using .NET 4.6.2.

Plugins or Workflow Activities should continue to be built using .NET Framework 4.5.2.

Please review [Blog Post: Updates coming to Dynamics 365 Customer Engagement connection security](https://blogs.msdn.microsoft.com/crm/2017/09/28/updates-coming-to-dynamics-365-customer-engagement-connection-security/) for full details.

## Integrate external data with Virtual Entities

You have a new way to integrate data from external systems. Without virtual
entities, common strategies to integrate external data include client-side code
to retrieve and display external data or server-side replication and
synchronization of external data within [!INCLUDE [pn-ms-dyn-365](../../../includes/pn-ms-dyn-365.md)] Customer Engagement. Virtual entities provide a
better approach for many external system data integration requirements.

More  information: [Get started with virtual entities](/dynamics365/customer-engagement/developer/virtual-entities/get-started-ve)

## Web API improvements

The following improvements are included in this release of the Web API, our
OData v4 endpoint:

-   Custom actions that return **EntityReference**, **Entity**, or
    **EntityCollection** types are available.

-   Changes to API behaviors are available using the latest v9.0 version of the
    service, legacy behaviors remain available in the v8.x version. You don’t
    have to change your code when you upgrade.

-   New messages: **GrantAccess**, **ModifyAccess**, and
    **RetrieveSharedPrincipalsAndAccess** messages are now available using the
    Web API.

-   We have made the amount of service metadata smaller by not including
    annotations by default. If you need the annotations, you can use parameters
    to have it included.

More information: [Use the Dynamics 365 Customer Engagement Web API](/dynamics365/customer-engagement/developer/use-microsoft-dynamics-365-web-api)

## Client API enhancements

With the introduction of [Unified Interface](./new-in-version-9.md#unified-interface-framework-for-new-apps) in the [!INCLUDE [pn-crm-9-0-0-online](../../../includes/pn-crm-9-0-0-online.md)] release, there are some significant changes made to the client APIs
to ensure that they work consistently across Unified Interface and the web
client.

### Using execution context to work with form and UI

One significant change is that now you use the execution content to retrieve the form context where you want to run your script instead of using the **Xrm.Page** object, which is deprecated in this release. More information: [Understand the Client API object model](/dynamics365/customer-engagement/developer/clientapi/understand-clientapi-object-model)

### Using global context
The [Xrm.Page.context](https://msdn.microsoft.com/en-us/library/gg334511.aspx)
that is used to reference the client-side context is deprecated in this release. You should now use new **Xrm.Utility.**[getGlobalContext](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-utility/getglobalcontext) method to retrieve the global context instead of going through the form context. The new method
contains an equivalent of all the methods available for the deprecated **Xrm.Page.context**
object to retrieve information specific to the organization, user, or client where the script is executed.

### New client APIs

We introduced a number of new client APIs in this release.

Here is a list of new namespaces in this release that contains new and some
existing methods that are moved under these namespaces for an enhanced object
model design.

| **New Namespace**  | **Description**                                                                                                                |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------|
| [Xrm.Device](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-device)     | Provides methods to use native device capabilities of mobile devices.                                                             |
| [Xrm.Encoding](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-encoding)    | Provides methods to encode strings.                                                    |
| [Xrm.Navigation](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-navigation) | Provides navigation-related methods. |
| [Xrm.WebApi](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-webapi)     | Provides properties and methods to use Web API to create and manage records and execute Web API actions and functions.|


The following new APIs were introduced in the existing namespaces:

| **Namespace**  | **New APIs** |
|--|--|
| [formContext.data](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-data) | - OnLoad event and even handlers (addOnLoad and removeOnLoad)<br/>- isValid<br/>- Updated saveOptions in the **formContext.data.save** method to include a new value called **saveMode** to let the onSave event handlers know why the save is happening<br/>- attributes collection|
| [formContext.data.entity](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-data-entity)           | getEntityReference<br/>isValid                                                                                                   |
| [formContext.data.entity attribute](/dynamics365/customer-engagement/developer/clientapi/reference/attributes) | isValid<br/>setPrecision                                                                                                                       |
| [formContext.ui](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-ui)                    | <!--setFormEntityName<br/>-->event handlers for the OnLoad event (addOnLoad and removeOnLoad)  |
| [Xrm.Utility](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-utility)                    | getAllowedStatusTransitions<br/>getEntityMetadata<br/>getGlobalContext<br/>getLearningPathAttributeName<br/>getResourceString<br/>invokeProcessAction<br/>lookupObjects</br>showProgressIndicator</br>closeProgressIndicator<br/>refreshParentGrid|
                                                                                                  

Apart from these new client APIs, there are some more client APIs introduced for
specific controls such as grids, lookup, optionset, and timer. For more information
about these new APIs, see [Controls](/dynamics365/customer-engagement/developer/clientapi/reference/controls).

### Deprecated client APIs

Some client APIs are deprecated, and you should use the new/improved client APIs
instead as mentioned in this list: [
Some client APIs are deprecated](./important-changes-coming.md#some-client-apis-are-deprecated)

**NOTE**: Deprecation means that we intend to remove the client API from any
future "major" release of [!INCLUDE [pn-ms-dyn-365](../../../includes/pn-ms-dyn-365.md)]. The client API will continue to work
and is fully supported until it is officially removed. After removal, the
feature or capability will no longer work. We are notifying you now so you have
sufficient time to plan and update your code before the feature or capability is
removed.

### Client API support for the new Timeline control in Unified Interface

The new Timeline control presents the Posts, Activities, and Notes in a unified
view. For information about client APIs supported for this control type, see [Controls](/dynamics365/customer-engagement/developer/clientapi/reference/controls#timelinewall%20control%20type)

## Create and manage role-based, purpose-built custom business apps

Business apps in [!INCLUDE [pn-ms-dyn-365](../../../includes/pn-ms-dyn-365.md)] are role-based, modular apps that provide
task-based functionality targeting a specific area of your business such as
sales, service, and marketing. These business apps provide a simple and
intuitive experience for users by enabling them to quickly navigate around, find
things easily, and perform their tasks effectively.

In addition to using the [app
designer](https://www.microsoft.com/en-us/dynamics/crm-customer-center/design-custom-business-apps-by-using-the-app-designer.aspx),
you can now programmatically create, manage, validate, and publish business
apps. While creating an app, you can select whether the app is for the web
client or [Unified Interface](./new-in-version-9.md#unified-interface-framework-for-new-apps).

More information: [Create and manage custom business apps in Customer Engagement using code](/dynamics365/customer-engagement/developer/create-manage-custom-business-apps-using-code)

## New attribute type: multi-select option set

Customizers can now define a new type of attribute that allows selection of
multiple options. Included in this work are new query condition operators to
write queries to retrieve data based on which options are selected. More information: [Multi-Select Picklist attributes](/dynamics365/customer-engagement/developer/multi-select-picklist)

### Form scripting support for multi-select option sets

Multi-select option sets are available for [Unified Interface](./new-in-version-9.md#unified-interface-framework-for-new-apps) and the
web client. Multi-select option sets are available for the following form
types: Main, Quick Create, and Quick View. Multi-select option sets won’t be
supported on legacy forms.

Multi-select option sets supports all the client APIs supported for the
    option sets
    [attributes](/dynamics365/customer-engagement/developer/clientapi/reference/attributes#multiselectoptionset-and-optionset-attribute-types)
    and
    [controls](/dynamics365/customer-engagement/developer/clientapi/reference/controls);
    the only difference is that the return value of certain methods will be an
    array instead of a single value.   

You can also set the value for multi-select option set fields for new records by specifying integer values for the options in the URL that is used to open the form. More information: [Example: Set the value for multi-select option set fields](/dynamics365/customer-engagement/developer/set-field-values-using-parameters-passed-form#BKMK_SampleSEtValueMultiSelectOptionSetFields)

## WebHooks integration

You will be able to integrate data from [!INCLUDE [pn-ms-dyn-365](../../../includes/pn-ms-dyn-365.md)] Customer Engagement to your own custom code
hosted on external services using WebHooks. You can use the plugin registration
tool to configure when to post Customer Engagement data to an external service.
WebHooks is a lightweight HTTP pattern for connecting Web APIs and services with
a publish/subscribe model. WebHooks senders notify receivers about events by
making requests to receiver endpoints with some information about the events. By
using the WebHooks model, you can secure your endpoint by using an
authentication header or query parameter keys. This provides an alternative to
the SAS authentication model that you may currently use for your Azure Service
Bus integration.

More information: [Use webhooks to create external handlers for server events](/dynamics365/customer-engagement/developer/use-webhooks)

## Vector Image web resources

Use vector images for any icon presented in the application. Vector images are
defined as Scalable Vector Graphics (SVG) an XML-based vector image format. The
advantage of vector images over other image web resources is that they scale.
You can define one vector image and re-use it rather than provide multiple sizes
of images. You can use this web resource to define a single icon for an entity
rather different sized images.

More information: [Image web resources](/dynamics365/customer-engagement/developer/image-web-resources)

## Support for localizable solutions

You can use RESX web resources to store localized strings for your solutions.
The RESX XML format is commonly used to define localized resources so there is
common tooling available to work with this type of file and localization vendors
will be familiar with working with them. You can associate RESX web resources
with any JavaScript web resource that uses them so that you can use a new
client-side API to access localized strings at runtime.

More information: [String (RESX) web resources](/dynamics365/customer-engagement/developer/resx-web-resources)

## JavaScript Web Resource dependencies

JavaScript web resources frequently need to interact with other resources which
can be other JavaScript libraries, images, attribute values, or the new RESX web
resource for localized strings. You can now configure a JavaScript web resource
to associate it with any dependent resources so that the resource is available
when needed.

When a JavaScript web resource is associated to another kind of web resource,
that web resource will be loaded automatically when the JavaScript web resource
is requested in the application. When a JavaScript web resource used in a form
script is associated to an attribute for a specific entity, that entity
attribute will be available to the script even when a field for that attribute
isn’t included in the form.

More information: [Web resource dependencies](/dynamics365/customer-engagement/developer/web-resource-dependencies)

## Interactive Service Hub improvements

These are the changes to the Interactive Service Hub:

- Interactive Service Hub is now called Customer Service Hub, and is available
  as a [Unified Interface](./new-in-version-9.md#unified-interface-framework-for-new-apps) app.

- The Customer Service Hub app uses the **Main** form type instead of the
  [Main - Interactive
  experience](https://technet.microsoft.com/library/mt622060.aspx) form type.
  If you upgrade from an earlier version of [!INCLUDE [pn-ms-dyn-365](../../../includes/pn-ms-dyn-365.md)] Customer Engagement, all your [Main -
  Interactive experience](https://technet.microsoft.com/library/mt622060.aspx)
  type of forms will be converted to the **Main** form type. Any of your
  customizable **Main - Interactive experience** type of forms will be set to
  inactive during the upgrade, and you must enable the converted forms after
  upgrade to use them. Also, all the **Main - Interactive experience** type of
  forms converted to the **Main** type of form will be ranked lower than the
  existing **Main** type of forms to prevent any [form
  order](https://technet.microsoft.com/en-us/library/dn531143.aspx#BKMK_FormOrder)
  conflicts. This ensures that the correct form is displayed to the users in
  web client post upgrade.

- All entities are now enabled for the interactive experience in the new
  Customer Service Hub app. This implies that the
  **EntityMetadata**.[IsInteractionCentricEnabled](https://msdn.microsoft.com/en-us/library/microsoft.xrm.sdk.metadata.entitymetadata.isinteractioncentricenabled.aspx)
  property, which indicates whether an entity can be enabled for interactive
  experience, is no longer relevant. The corresponding setting for this
  property in the Customization tool, **Enable for interactive experience**,
  is removed in the current release, and the
  **EntityMetadata**.[IsInteractionCentricEnabled](https://msdn.microsoft.com/en-us/library/microsoft.xrm.sdk.metadata.entitymetadata.isinteractioncentricenabled.aspx)
  property will be removed from the future version of [!INCLUDE [pn-sdk](../../../includes/pn-sdk.md)] for Customer
  Engagement.

## Override the default open behavior of data rows in an entity-bound grid

Currently, performing any of the following actions in a data row in an
entity-bound grid opens the entity record by default:

-   Double-clicking the data row or clicking the primary attribute link in the
    row.

-   Selecting a data row, and pressing ENTER.

-   On a touch-enabled device, selecting a data row.

There might be situations where you do not want the entity record to open, such
as, for document management records, you might want to open a SharePoint site
instead of displaying the record. You can now override the default behavior to
define your own custom behavior.

You can now create a command definition for an entity with
**Mscrm.OpenRecordItem** as the value of the **Id** attribute
([\<CommandDefinition\>
(RibbonDiffXml)](https://msdn.microsoft.com/library/gg334414.aspx)), and define
custom action for the command [\<Actions\>
(RibbonDiffXml)](https://msdn.microsoft.com/en-us/library/gg328038.aspx).
Customer Engagement will look for this command Id for an entity when you try to open a
record from the entity-bound grid, and if present, will execute the custom
action instead of opening the entity record (default behavior).

> [!NOTE]
> This feature is supported only for [Unified Interface](./new-in-version-9.md#unified-interface-framework-for-new-apps).

## Business process flow enhancements

Business process flows has been enhanced to offer the following changes:

- On Unified Interface, the
  [setDisplayState](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-ui-process/setdisplaystate)
  method now lets you set a business process control in the “floating” state,
  in addition to “expanded” and “collapsed.” Similarly, the
  [getDisplayState](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-ui-process/getdisplaystate)
  method can return “floating”, “expanded” or “collapsed” depending on the
  state of a business process control. The floating state is not applicable for the web client.

- You can now run process actions using the new client API: **Xrm.Utility**.[invokeProcessAction](/dynamics365/customer-engagement/developer/clientapi/reference/xrm-utility/invokeprocessaction). The ability to programmatically run process actions using the new client API is released as a preview feature in this release. On the web client, you can run any process action using the new client API. However, on Unified Interface, only those process actions that are available to run as a business process step can be run using the new client API.

- Get and set the progress of a process action step using the new client APIs: [getProgress](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-data-process/step/getprogress) and [setProgress](/dynamics365/customer-engagement/developer/clientapi/reference/formcontext-data-process/step/getprogress). Process action steps are buttons on the business process stages that users can click to trigger an on-demand workflow or action. Process action step is a preview feature introduced in the [!INCLUDE [pn_crm_9_0_0_online](../../../includes/pn-crm-9-0-0-online.md)] release. More information: See the **Business Process Flow automation with Action Steps** section in [Blog: New automation and visualization features for Business Process Flows (public preview)](https://blogs.msdn.microsoft.com/crm/2017/10/25/new-automation-and-visualization-features-for-business-process-flows-public-preview/).

  >[!NOTE]
  >The **getProgress** and **setProgress** client APIs aren’t supported for the process data step.

## See also

[What's new in Unified Service Desk for developers and customizers](/dynamics365/customer-engagement/unified-service-desk/what-s-new-in-unified-service-desk)

[Developer Guide for Dynamics 365 Customer Engagement](/dynamics365/customer-engagement/developer/developer-guide)



