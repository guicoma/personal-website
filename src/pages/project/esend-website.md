---
title: "eSend - Web App"
date: 2023
techStack: "React.js, Typescript, antd"
layout: "../../layouts/project.astro"
href: "http://esend.es"
---

An online platform to send and receive files amongst users. A cloud-based file transfer service based on end-to-end ciphering, utilizing the crypto library libsodium.

This project is an alternative to other popular file sharing platforms such as weTransfer. Although at first sight it seems a B2C model, the intention was make an application for business to have an inhouse solution for sensitive document sharing. Being able to host and manage their data on their servers, handling the access to their files. A backoffice section was implemented for businesses to be able to add users, adjust limitations to sharing options.

Here are the configurations features implemented for the file sharing application:

- **Password protection**:
A user is able to apply a password to add an extra layer of security to the data being transfered. The sender may also add a *hint* to facilitate the receiver a way to recall the password that is being applied. This also limits visibility in the backoffice side of the application, since one can only decipher the transfer with the password. Some metadata is stored publically, such as size and number of items.
- **Limit downloads**: This allows the user to set a maximum number of downloads of the transfer.
- **Expire access**: Another common feature seen in these kind of applications, where the send can set a time window to access the transfer. In this case it is only set to several options such as 1 day, 2 days, weeks or to never *expire*. By default, to avoid storage saturation, it is set to 2 weeks.
- **Notify first access**: If activated, the sender will be notified when the receiver opens the transfer for the first time.

I was assigned the task to design and implement the frontend side of both the main page and the backoffice part.
This project has gone through several rewrites, updating libraries and other refactors.

The technologies used are [React](https://react.dev/) utilizing the frontend tooling [Vite](https://vite.dev/) and the React UI framework [Ant Design](https://ant.design/).