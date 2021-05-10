# File Server

One of the key aims of the FutureNHS Platform is to make it as simple as possible to promote collaborative discussion over common file types such as Microsoft Office documents and PDF.

Files can be attached at various extension points within the system and used to promote/aid discussion or as a point of record:

* To a discussion thread within a group
* To a group's document repository

Files can of course be uplodaed, downloaded, versioned, viewed, edited, commented upon and archived.  They can be logically grouped alongside other files within a 'Document' structure and are fully audited and protected by role-based permissions.

## In-Browser File View & Edit

One of the key goals of the platform is to empower third parties to standup their own variant, while asking them to take minimal dependencies on commercial products.  Unfortunately, the in-browser file editing/viewing space has proven quite a challenge in this respect and FutureNHS have had to [move forward with a licensed product](..\decisions\0003-file-viewer).  Because of this, rather than stand up an open-source file server we decided to build our own, and to do so using open protocols such as WOPI.  This decision means the range of 'clients' the platform can extend to interact with is theoretically unlimited and thus it is hoped over time, contributors will add support for a number of different 'clients' to handle all file viewing/editing while the file server takes care of managing things.  

FutureNHS have so far settled upon [Collabora Online](https://github.com/CollaboraOnline/online), but continue to progress talks with Microsoft to add support for [Office Web Apps](https://www.office.com/).

Other products which we investigated, and would like to extend support to in the future, include [Aspose](https://www.aspose.com/) and [OnlyOffice](https://www.onlyoffice.com/).

## File Sensitivity

Please visit [here](sensitive-files.md) for more information.

