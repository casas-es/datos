# Datos abiertos de CASAS.ES

Cifras de los municipios y las calles de España, calculadas por [CASAS.ES](https://casas.es/) con datos de la
Dirección General del Catastro, el INE y el Instituto Geográfico Nacional.

**Web:** https://casas-es.github.io/datos/

## Qué hay

| Fichero | Qué es | Filas |
|---|---|---|
| [`datos/malaga-municipios.csv`](datos/malaga-municipios.csv) | Los 103 municipios de la provincia de Málaga | 103 |
| [`datos/malaga-calles.csv`](datos/malaga-calles.csv) | Las calles con más viviendas de cada municipio de Málaga, con su página en CASAS.ES | 958 |

**Solo hay cifras de municipios y calles enteros.** No hay nada de un edificio concreto, ni titulares, ni valores
catastrales.

### `malaga-municipios.csv`

| Columna | Qué es |
|---|---|
| `ine` | Código INE del municipio, cinco cifras |
| `municipio`, `provincia` | Nombres |
| `edificios`, `viviendas` | Edificios y viviendas según el Catastro |
| `habitantes`, `anio_habitantes` | Población del padrón (INE) y su año |
| `mediana_anio_construccion` | La mitad de los edificios es de ese año o posterior |
| `pct_antes_1960`, `pct_1960_1979`, `pct_1980_1999`, `pct_desde_2000` | % de edificios construidos en cada época; suman 100 |
| `pct_anteriores_1979` | % de edificios anteriores a 1979, año de la primera norma térmica (NBE-CT-79) |
| `edificios_desde_2015` | Edificios terminados desde 2015 |
| `edificios_anteriores_1900` | Edificios anteriores a 1900 |
| `calles` | Número de calles del municipio |
| `costa` | `sí` en los 14 municipios con mar |
| `url_casas_es` | Página del municipio en CASAS.ES |
| `wikidata` | Elemento del municipio en Wikidata |
| `url_datos_abiertos` | Página del municipio en esta web |

### `malaga-calles.csv`

| Columna | Qué es |
|---|---|
| `ine`, `municipio` | El municipio |
| `puesto` | Puesto de la calle por número de viviendas dentro del municipio |
| `calle` | Nombre de la calle |
| `viviendas` | Viviendas de la calle según el Catastro |
| `url_casas_es` | Página de la calle en CASAS.ES |

## Fuentes

- **Edificios, viviendas y año de construcción:** Dirección General del Catastro. En los edificios más antiguos, el
  año del Catastro es a menudo aproximado.
- **Habitantes:** padrón municipal, INE.
- **Fotos aéreas:** Vuelo Americano Serie B (1956–57) y PNOA, cedidos por © Instituto Geográfico Nacional, CC BY 4.0
  scne.es.
- **Cómo se calcula cada cifra:** https://casas.es/metodologia

## Licencia

[CC BY 4.0](LICENSE). Puedes copiar, reutilizar y adaptar estos datos, también con fines comerciales, citando:

> CASAS.ES, con datos de la Dirección General del Catastro, el INE y el Instituto Geográfico Nacional.

## Actualizaciones

- **31-oct-2026:** primera versión, con la provincia de Málaga.
