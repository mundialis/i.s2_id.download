# i.s2_id.download

## DESCRIPTION

*i.s2_id.download* downloads a Sentinel-2 Level-2A scene from Copernicus
Data Space by scene ID using [EODAG](https://eodag.readthedocs.io/).

The module searches for the given scene ID and downloads the product when a matching product is found.

Search and download are configured for:

- Preferred provider: `Copernicus Data Space Ecosystem (CDSE)`
- Collection: `S2_MSI_L2A`

## EXAMPLES

### Download a scene to an existing directory

```sh
i.s2_id.download \
    s2_id=S2B_MSIL2A_20240109T103329_N0510_R108_T32ULB_20240109T114910 \
    download_dir=/path/to/download_dir
```

## NOTES

- Requires a working EODAG installation.
- For `CDSE`, make sure authentication is configured in EODAG.
- If no match is found for `s2_id`, no download is performed.
- Downloaded archive is not automatically extracted.

## SEE ALSO

- [EODAG installation](https://eodag.readthedocs.io/en/stable/getting_started_guide/install.html)
- [CDSE](https://dataspace.copernicus.eu/)
- [STAC specification](https://stacspec.org/en)

## AUTHOR

Jonas Pischke, [mundialis GmbH & Co. KG](https://www.mundialis.de/), Germany
