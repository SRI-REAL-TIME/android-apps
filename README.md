# SRI REAL TIME — Android apps

Public download host for SRI REAL TIME Android builds. The apps are listed,
with download buttons and QR codes, at **https://srirealtime.com/apps**.

This repository holds no source code — only the release files. Each release
carries the APKs under fixed names, and the website links to
`releases/latest/download/<file>`, so publishing a new release is all it takes
to ship an update:

| File | App |
| --- | --- |
| `pasumaivelanmai.apk` | Pasumaivelanmai — for farmers |
| `pv-seller.apk` | PV Seller — for sellers and manufacturers |
| `badaga-matrimony.apk` | Badaga Matrimony |

```sh
gh release create v<date> --repo SRI-REAL-TIME/android-apps --title "<date>" \
  pasumaivelanmai.apk pv-seller.apk badaga-matrimony.apk
```

Every new release must include **all** the files above — `latest` points at
one release, so a file missing from it stops downloading.
