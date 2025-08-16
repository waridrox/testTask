# Species Assembly Viewer
A web app built with vanilla JS, HTML and CSS that displays genome assembly info for various species using the Ensembl REST API.

## Usage
1. Open `index.html` in any web browser.
2. Select a species from the dropdown menu.
3. View the assembly information including species name, total genome length and individual chromosome lengths

### Data Formatting
- Genome lengths are displayed in appropriate units (bp, Kb, Mb)
- Chromosomes are sorted in karyotype order (1-22, X, Y, MT)

## API Calls
- [Species Endpoint](https://rest.ensembl.org/documentation/info/species)
- [Assembly Endpoint](https://rest.ensembl.org/documentation/info/assembly)

```bash
curl 'https://rest.ensembl.org/info/species?' -H 'Content-type: application/json'

curl 'https://rest.ensembl.org/info/assembly/homo_sapiens?' -H 'Content-type: application/json'
```
