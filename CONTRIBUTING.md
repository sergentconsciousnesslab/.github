# Contributing guidelines

These guidelines should be applied by members and collaborators working on the repositories of the Sergent Consciousness Lab organization.

<!-- TODO: decide whether issues and pull requests from external contributors are accepted -->

## Data and confidentiality

- Datasets are stored outside GitHub on the institutional server, while repositories only reference their location.
- No participant or patient data may be committed to any repository, whether raw or pseudonymized, including identifiers, consent documents, and clinical information.
- No credentials may be committed: passwords, access tokens, API keys, private keys.

<!-- TODO: name the storage location or archive for datasets (e.g. institutional server) -->

> [!IMPORTANT]
> If such content is committed by mistake:
>
> 1. notify the maintainer,
> 2. revoke any exposed credential,
> 3. purge the content from the commit history.
>
> Deleting the file in a later commit is *not sufficient*.

<!-- TODO: name the maintainer to notify -->

## Reproducibility and open science

- The version of the code used for a publication is identified by a tag or release.
- Code associated with a publication must allow every figure and result to be regenerated, following a documented procedure.

<!-- TODO: decide whether releases associated with a publication are archived with a DOI, and where (e.g. Zenodo, Software Heritage) -->
<!-- TODO: decide when a study repository is made public (at preprint, at publication) and whether it is archived (read-only) afterwards -->

## Credit

Every repository should:

- select a license and ship it in a `LICENSE` file,
- provide a `CITATION.cff` file at its root, listing the authors of the code and, once published, the associated article as the preferred citation.

<!-- TODO: decide the default license (e.g. MIT or BSD-3-Clause for code, CC BY 4.0 for documentation and figures), after checking CNRS and Université Paris Cité policy -->

## Repository requirements

Every repository should contain:

- a `README.md` file stating at least the purpose of the repository, how to install the environment, and how to run the code,
- a pinned environment specification (e.g. `environment.yml`, `requirements.txt`, `pyproject.toml` with a lock file),
- a `.gitignore` file excluding data files, outputs, and local configuration.

## Naming and file system

<!-- TODO: decide the repository naming pattern, for instance lowercase, hyphenated, with a type prefix:
       study-<short-name>           code reproducing an article or preprint
       experiment-<short-name>      experimental paradigms and stimulus presentation
       tool-<short-name>            shared libraries and pipelines -->
<!-- TODO: decide the list of topics to set on repositories (e.g. eeg, meg, fmri, modelling) -->
<!-- TODO: decide the standard directory structure per repository type -->

## Workflow

- The default branch contains working code.
- Commit messages should follow the [Conventional Commits specification](https://www.conventionalcommits.org/en/v1.0.0/), using the organization's [commit message template](https://github.com/ORG/.github/blob/HEAD/.gitmessage).

> [!TIP]
> To enable the template, download it and register it once:
> ```bash
> git config --global commit.template ~/.gitmessage
> ```

<!-- TODO: decide the branching model (e.g. short-lived feature branches merged through pull requests) -->

## Code standards

<!-- TODO: decide the supported languages -->
<!-- TODO: decide whether testing, formatter and linter are enforced through pre-commit hooks or continuous integration -->
<!-- TODO: decide the documentation style (e.g. docstring convention) -->

## Contact

Questions about these guidelines can be addressed to [Esther Poniatowski](mailto:esther.poniatowski@u-pariscite.fr).
