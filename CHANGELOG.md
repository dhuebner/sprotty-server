## Eclipse Sprotty Change Log (Server)

This change log covers only the server part of Sprotty. See also the change logs of [sprotty](https://github.com/eclipse/sprotty/blob/master/CHANGELOG.md), [sprotty-theia](https://github.com/eclipse/sprotty-theia/blob/master/CHANGELOG.md) and [sprotty-layout](https://github.com/eclipse/sprotty-layout/blob/master/CHANGELOG.md).

### v0.12.0 (Jun. 2022)

New features:
 * Dependencies update


-----

### v0.9.0 (Aug. 2020)

New features:
 * Support request rejection ([#78](https://github.com/eclipse/sprotty-server/pull/78))

Fixed issues: https://github.com/eclipse/sprotty-server/milestone/3?closed=1

-----

### v0.8.0 (Apr. 2020)

New features:

* Center action retains zoom level ([#58](https://github.com/eclipse/sprotty-server/pull/58))
* Build OSGi compliant jars ([#62](https://github.com/eclipse/sprotty-server/pull/62))
* Upgrade to Xtext 2.21 ([#67](https://github.com/eclipse/sprotty-server/pull/67))

Fixed issues: https://github.com/eclipse/sprotty-server/milestone/2?closed=1

-----

### v0.7.0 (Oct. 2019)

New features:

 * Request-response actions ([#34](https://github.com/eclipse/sprotty-server/pull/34))
 * Example using WebSocket ([#34](https://github.com/eclipse/sprotty-server/pull/34))
 * New class `ElktSerializer` for serializing ELK graphs ([#47](https://github.com/eclipse/sprotty-server/pull/47))
 * New classes `SModelIterator` and `SModelIterable` ([#56](https://github.com/eclipse/sprotty-server/pull/56))
 * Cleaned up handling of client/server-side layout ([#41](https://github.com/eclipse/sprotty-server/pull/41), [#52](https://github.com/eclipse/sprotty-server/pull/52))

Fixed issues: https://github.com/eclipse/sprotty-server/milestone/1?closed=1

Breaking API changes:

 * `DefaultDiagramServer.submitModel` requires an additional parameter `cause` ([#34](https://github.com/eclipse/sprotty-server/pull/34))
 * `ILayoutEngine.layout` requires an additional parameter `cause` ([#36](https://github.com/eclipse/sprotty-server/pull/36))
 * `ElkLayoutEngine.transformGraph` requires an additional parameter `cause` ([#41](https://github.com/eclipse/sprotty-server/pull/41))
 * Extracted application of bounds to new service `ComputedBoundsApplicator` (replaces `LayoutUtil`) ([#41](https://github.com/eclipse/sprotty-server/pull/41))
 * Changed `ComputedBoundsAction` ([#41](https://github.com/eclipse/sprotty-server/pull/41))
 * Removed `ServerLayoutKind` ([#41](https://github.com/eclipse/sprotty-server/pull/41))
 * The client now decides whether to apply layout on client-side as well as server-side ([#52](https://github.com/eclipse/sprotty-server/pull/52))
 * Removed `DefaultDiagramServer.setNeedsClientLayout` ([#52](https://github.com/eclipse/sprotty-server/pull/52))

-----

### v0.6.0 (Mar. 2019)

First release of Sprotty with the Eclipse Foundation. The previous repository location was [theia-ide/sprotty](https://github.com/theia-ide/sprotty) (Maven group id: `io.typefox.sprotty`).
