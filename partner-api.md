# Partner API doc

To access partner API you need to partner API key in `Authorization: Bearer` header.
To get API key please contact Cosmo Bear team, example of key: `cb_H1WXCMUB334YXIMLZCRQB6UKS1935C62680ZDYTF`

Request example:
```bash
curl -v --location "https://cosmobear.io/api/partner/v1/user?id=340744037"\
 --header 'Authorization: Bearer cb_XXX...'
```

Response example:
```json
{
  "is_registered": true,
  "from_partner": true
}
```

`id` **required** - Telegram user ID (integer)

`is_registered` - identifies if user started bot or app
`from_partner` - identifies if user came from partner to whom the API key belongs or was present in DB earlier.
