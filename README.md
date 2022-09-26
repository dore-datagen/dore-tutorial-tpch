# Dore Tutorial

This repository contains files which form the TPC-H Dore manifest.

You can choose to either clone this repo or download the files as a .zip archive.

## Usage

We can invoke Dore with the `tpch-mysql-manifest.json` manifest from this repo
after making a few changes to the Datastore file at `tpch-mysql-datastore.json`.

* Replace `"<mysql-host>"` with actual MySQL host.

* Replace `"<mysql-port>"` with actual MySQL port.

Once these changes are done, you can invoke Dore with the Manifest as follows:

```bash
$ dore --manifest /abs/path/to/tpch-mysql-manifest.json \
  --project-dir=/abs/path/to/project_directory
  --mysql-username=<your mysql username> \
  --mysql-password=<your mysql password>
```

**Note: ** Value for `--project-dir` should be *absolute path* to this repository's location on your machine.
