# Amazion Route53 Dynamic DNS Updater

This project leverages Route53 API to provide dynamic DNS on domain A (alias) records.

## Setup
As indicated by the Area53 documentation, need to set the following environment variables:

```bash
export AWS_ACCESS_KEY_ID="<Insert your AWS Access Key>"
export AWS_SECRET_ACCESS_KEY="<Insert your AWS Secret Key>"
```

## Use
```Usage: r53dyndns.py --record=RECORD_TO_UPDATE --url=IP_GET_URL```

## Dependencies :

+   A URL that returns the client IP alone in plaintext. No support is included for other standard services.
+   Area53 interface : https://github.com/mariusv/Area53.git
+   boto : https://github.com/boto/boto