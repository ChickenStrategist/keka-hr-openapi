# Keka HR API

Official OpenAPI 3.0 specification for Keka HR API integration with Rewst.

## Documentation
[Rewst Custom Integration Guide](https://docs.rewst.help/documentation/configuration/integrations/custom-integrations/custom-integrations-v2)

## Specification Details
- **Version**: 1.0.0
- **Base URL**: `https://{company}.{environment}.com/api/v1`
- **Authentication**: OAuth2

## Description
Keka is a leading human resources management system that enables organizations to seamlessly manage diverse aspects of their human resource processes, including recruitment and onboarding, attendance and time management, payroll, expense and performance management.

With OAuth authentication, rate limiting, pagination, and adherence to industry standards, Keka provides developers with everything they need to build robust integrations with their software/platform and facilitate data exchange between their application and this leading HRMS portal.

**Rate Limiting:** 50 API requests per minute
**Pagination:** Default page size is 100, default page number is 1
**Environment:** Sandbox available at signup.keka.com

## Usage

### Import into Rewst
1. Navigate to: Rewst Dashboard > Configuration > Integrations
2. Create Custom Integration
3. Upload `openapi.json` from this repository
4. Configure authentication parameters
5. Test connection

### Import into API Testing Tools
- **Postman**: Import > Link > Paste raw GitHub URL
- **Insomnia**: Import > URL > Paste raw GitHub URL
- **OpenAPI Generator**: `openapi-generator-cli generate -i openapi.json`

## Repository Structure
```
.
├── openapi.json              # Primary OpenAPI 3.0 specification
├── assets/                   # Integration assets (logos, guides)
├── README.md                 # This file
└── .github/
    └── workflows/
        └── validate-openapi.yml  # CI validation
```

## Validation
This specification is automatically validated on every commit using GitHub Actions.

## Contributing
Maintained by Rewst APAC Automation Team.

## Support
- **Technical Support**: roc@rewst.io
- **Documentation**: [Rewst Docs](https://docs.rewst.help)

## License
Private repository - Rewst LLC internal use only.
