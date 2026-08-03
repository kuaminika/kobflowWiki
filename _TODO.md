kobflow-wiki/
├── README.md              — entry point: what Kobflow is, links to all repos, how to navigate this wiki
├── repos.md                — map of all repos in the project and what each one owns
├── domain/
│   ├── entities.md         — expenses, incomes, categories, sources, merchants, kobholders
│   └── relationships.md    — how entities relate to each other
├── architecture/
│   ├── command-pattern.md  — HandleAddCommand refactor
│   ├── components.md       — ManageList, ListLoader, KCacher
│   └── merchant-mapping.md — MerchantMappingController
├── conventions/
│   ├── code-style.md       — options-objects, arrow fns vs self=this, self.execute pattern
│   └── patterns-under-debate.md — constructor fn vs plain fn, etc.
├── decisions/
│   └── 0001-example.md     — lightweight ADR log, one file per decision
├── setup/
│   ├── dev-containers.md
│   └── claude-code.md      — CLAUDE.md rules, Plan Mode workflow
└── project-tracking.md     — how Linear (Kuaminika team) maps to this wiki
clients/
├── web.md        — react website: stack, structure, conventions
└── mobile.md      — ionic app: stack, structure, conventions