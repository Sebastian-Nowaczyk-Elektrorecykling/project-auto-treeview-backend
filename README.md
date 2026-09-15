# Treeview backend

Dependency-free Node.js implementation of the Project Auto Treeview contract.
It stores a recursively nested tree, validates every replacement, and rejects
stale writes through an integer revision.

## Run

```sh
npm start
```

The service listens on `http://localhost:8787`. Set `PORT`, `HOST`,
`TREE_DATA_FILE`, or `CORS_ORIGIN` to override its defaults. Data is persisted
to `var/tree.json` using write-then-rename replacement.

```sh
npm test
```

This implements contract version `0.1.0` from
`project-auto-treeview-contract`. Merge the contract PR first.
