# Soracom LPWAN Coverage

Soracom maintains an official list of [Supported Carriers](https://developers.soracom.io/en/docs/reference/carriers/) that provides up-to-date details of its global cellular coverage. While this list represents cellular network coverage that is guaranteed through Soracom's roaming contracts and partnerships, there are many additional cellular networks where network access is available to devices using Soracom IoT SIMs but which are not yet officially guaranteed.

This repository provides supplemental information regarding testing that Soracom has performed for these additional cellular networks. Where testing is possible, each of the cellular networks listed in this repository are tested several times to confirm that data transfer is possible.

## Test information

- `Guaranteed` indicates a network where coverage is guaranteed through a roaming agreement.
- `Validated` indicates a network that has been independently tested and proven to function at the time of the test. These networks are not covered by a contract, and no SLA is provided.
- `Observed` indicates a network where traffic other related activity has been identified but currently cannot be independently tested and verified. Similarly, these networks are not covered by a contract, and no SLA is provided.

Please note that these test results are subject to inaccuracies as a result of changes to roaming agreements or technical modifications by the network operator to the network itself.

## Legend

The list of networks and their corresponding coverage test is provided as a CSV file with the following fields:

```plaintext
Country, ISO3166    Tested country and ISO-3166 3-letter country code
MCC MNC             Mobile Country Code (3 digits) & Mobile Network Code (2-3 digits)
MNO                 Mobile Network Operator name (corresponding to the name listed on the Supported Carriers page)
RAT                 Radio Access Technology (LTE-M or NB-IoT)
Bands (Main)        LTE bands used for the test (additional bands may not be listed even if available)
Plan                The Soracom IoT SIM subscription plan used for the test
Support             Result of the test:
                      - Guaranteed: Coverage is provided with roaming agreement (also shown on Supported Carriers page)
                      - Validated: Coverage is still under testing and deployment; Coverage and compatibility is subject to change
                      - Observed: Related traffic was identified but coverage has not yet been independently tested and verified
Supported Features  Network features tested:
                      - All networks are tested for data transfer
                      - Where applicable, Low Power Wide Area Network (LPWAN) features such as eDRX, PSM and SMS are also tested
                        - eDRX* and PSM* (with asterisk) indicates that a requested eDRX or PSM value will be modified by the local MNO
Date                The most recent date that the test was performed
```

## Related subscription plans

The test results for the these subscription plans also apply to the following subscription plans:

- Test results for `plan01s` also apply to `plan01s - LDV` and `plan-NA1`
- Test results for `planX3` also apply to `planX3-EU`
- Test results for `planP1` also apply to `plan-US-NA`

However, please note that coverage for each of these related subscription plans may differ. Refer to the [Supported Carriers](https://developers.soracom.io/en/docs/reference/carriers/) page.

## Additional resources

- Soracom [Supported Carriers](https://developers.soracom.io/en/docs/reference/carriers/)
- Soracom [PSM Calculator](https://www.soracom.io/psm-calculation-tool/)

Further information regarding LPWAN features:

- [GSMA 1](https://www.gsma.com/solutions-and-impact/technologies/internet-of-things/wp-content/uploads/2022/04/LTE-M-Roaming-Features-April-2022-Landscape.pdf)
- [GSMA 2](https://www.gsma.com/iot/wp-content/uploads/2021/12/Mobile-Operator-LTE-M-Settings.pdf)
- [IoTcreators LTE-M](https://files.readme.io/68df4f3-Feature_matrix_LTE-M_20220830.png)
- [IoTcreators NB-IoT](https://files.readme.io/698ddd5-Feature_matrix_NB-IoT_20230814.png)

---

## Legal Disclaimer

The purpose of this page and all related files ("Coverage Documentation") is to provide our customers with the most up-to-date information regarding the status of our available networks and features.

NOTWITHSTANDING ANYTHING TO THE CONTRARY IN THE COVERAGE DOCUMENTATION, ALL INFORMATION CONTAINED THEREIN IS PROVIDED "<ins>**AS-IS**</ins>". WE DISCLAIM ALL WARRANTIES, EXPRESS AND IMPLIED, REGARDING SUCH INFORMATION, INCLUDING ALL WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE, NON-INFRINGEMENT OF INTELLECTUAL PROPERTY RIGHTS, AND ACCURACY OR UTILITY. WE WILL NOT HAVE ANY LIABILITY RESULTING FROM YOUR USE OR RELIANCE ON SUCH INFORMATION.

Furthermore, we reserve the right to make changes to the Coverage Documentation from time to time without notice.
