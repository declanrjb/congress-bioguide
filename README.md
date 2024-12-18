The [U.S. Congressional Bioguide](https://bioguide.congress.gov/) provides extensive biographical information on the elected members of each United States Congress and Continental Congress since 1774. This repository standardizes that data into four tidy tables for ease of analysis. The following tables are included in `congressional-bioguide.zip`:

## directory
Biographical information for each individual elected to the United States or Continental Congress, with one row per individual. Includes the following fields:

| Field | Description |
| ----- | ----------- |
| usCongressBioId | Unique serial of the elected representative. |
| fullName | Representative's given name followed by their family name, separated by a space. Representative's middle name not included. |
| givenName | Representative's given name. |
| middleName | Representative's middle name. |
| familyName | Representative's family name. |
| birthDate | Representative's birth date in YYYY-MM-DD format. |
| birthCirca | |
| deathDate |  Representative's death date in YYYY-MM-DD format. |
| deathCirca | |
| profileText | Narrative biography of the representative's life, notable events, and career accomplishments, in plain text. Clauses/events are typically separated by semicolons. |

## research-materials
Physical artifacts and papers of interest to historians and researchers pursuing work related to a given representative. Includes the following fields:

| Field | Description |
| ----- | ----------- |
| usCongressBioId | Unique serial of the elected representative. |
| representativeName | Representative's given name followed by their family name, separated by a space. Representative's middle name not included. |
| recordName | Name of the artifact, set of papers, or other material. |
| recordType | Specifies the medium in which the record is preserved. Includes papers, microfilm, and photographs, among others. |
| recordDescription | Narrative description of the record and its contents. |
| recordLocationName | Name of the library, archive, or other location at which the record is stored. |
| recordLocationAddress | City and U.S. state in which the record is currently stored. |

## congressional-positions
Terms and positions held by each member within congress, with one row per term. usCongressBioIds are used to uniquely identify individuals and may repeat.

| Field | Description |
| usCongressBioId | Unique serial of the elected representative. |
| representativeName | Representative's given name followed by their family name, separated by a space. Representative's middle name not included. |
| congressID | Unique ID for a given session of the US or Continental Congress. |
| jobName | The type of job held by the elected individual during the given term (Representative, Senator, Speaker, etc.) |
| jobType | Type of position held. Includes 'CongressMemberJob', 'CongressLeadershipJob', and 'OtherJob'. |
| stateRepresented | The U.S. State or territory the elected official represented during the given term. |
| party | The official's political party affiliation during the given term. |
| caucus | The official's caucus affiliation during the given term. |
| jobStartDate | The date on which the official began serving their term. |
| jobStartCirca | |