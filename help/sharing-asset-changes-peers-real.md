---
title: Sharing asset changes with peers in real time
seo-title: Sharing asset changes with peers in real time
description: null
seo-description: Learn how to share asset changes with peers in real time.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be

---

# Sharing asset changes with peers in real time{#sharing-asset-changes-with-peers-in-real-time}

With multiple copies of Scene7 running on one or more computers in the same company, the following actions from any Scene7 client are updated in real-time with all peer clients:

* Edit an asset (builder, image editor, etc.)
* Rename an asset
* Delete an asset
* Move an asset
* Upload one or more assets (both desktop and FTP)
* Create, delete, or rename a folder

After a change is made in the originating client, all peer clients logged into the same company are updated with the change. Changes are made to peers without notification, unless the peer is editing a changing asset in any of the image editors or builders.

When you log in, Flash Player prompts you to allow or deny peer updates. You can "remember" the choice so you are only prompted once. To clear your choice, delete the appropriate site from the Peer Assisted Networking panel in Global Settings.

If you are editing an asset that is changed by a peer, you are prompted to ingest the change into the builder or editor. If you choose Yes, then the builder or editor discards any changes made to the asset and imports the updated asset. If you choose No, the asset is unchanged in the builder or editor and any changes you’ve made persist in that session.

When you save the asset, you are notified that a newer version exists and asked if you want to overwrite the asset with your changes.
