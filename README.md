# France Company Search (SIREN / SIRET) MCP

Search French companies by name or SIREN and open company profiles with the head-office SIRET, legal category, creation date and status.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/company/france
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month

## France data coverage

- Company ids are `FR` + the 9-digit SIREN, e.g. `FR330033069`
- Head-office SIRET, legal category (catégorie juridique), creation date and active / closed status
- Activity (NAF) code where available

## Example prompts

- *"Look up SIREN 330033069"*
- *"Find active French companies with 'Danone' in the name"*
- *"What is the legal category and creation date of this SAS?"*
- *"List closed companies named 'Boulangerie du Centre'"*

## Tools

| Tool | Description |
|---|---|
| `France_search_companies` | Search companies in the France registry by name or id |
| `France_get_company` | Full company profile by id (the `FR` prefix is optional) |

## Français

Les données du répertoire SIRENE pour votre assistant IA : recherchez une entreprise par nom ou numéro SIREN, et consultez sa fiche avec le SIRET du siège, la catégorie juridique, la date de création et le statut (active ou fermée).

**Exemples de questions**

- *"Recherche le SIREN 330033069"*
- *"Trouve les entreprises actives dont le nom contient 'Danone'"*
- *"Quelle est la catégorie juridique de cette SAS ?"*

## Keywords

SIREN, SIRET, recherche entreprise, numéro SIREN, fiche entreprise, registre du commerce, Pappers alternative, Societe.com alternative
