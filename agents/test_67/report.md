# File Structure Report — Bench_GitHub_MCP & Bench_GitHub_MCP2

Generated: 2026-08-06

## Repository: Bench_GitHub_MCP

```
Bench_GitHub_MCP/
├── README.md
└── agents/
    ├── Report.md
    ├── test_27.md
    ├── test_28.md
    ├── test_29.md
    ├── test_30.md
    ├── test_31.md
    ├── test_32.md
    ├── test_33/report.md
    ├── test_34/report.md
    ├── test_35/report.md
    ├── test_36/report.md
    ├── test_37/report.md
    ├── test_38/report.md
    ├── test_39/report.md
    ├── test_40/report.md
    ├── test_41/report.md
    ├── test_42/report.md
    ├── test_43/report.md
    ├── test_44/report.md
    ├── test_45/report.md
    ├── test_46/report.md
    ├── test_47/report.md
    ├── test_48/report.md
    ├── test_49/report.md
    ├── test_50/report.md
    ├── test_51/report.md
    ├── test_52/report.md
    ├── test_53/report.md
    ├── test_54.md
    ├── test_55/report.md
    ├── test_56/report.md
    ├── test_57/report.md
    ├── test_58/report.md
    ├── test_59/report.md
    ├── test_60/report.md
    ├── test_61/report.md
    ├── test_62/report.md
    ├── test_63/report.md
    ├── test_64/report.md
    ├── test_65/report.md
    └── test_66/report.md
```

**Summary:** Root contains `README.md` and an `agents/` folder. Inside `agents/`, tests 27–32 and 54 are flat `.md` files, while tests 33–53 and 55–66 are each a subfolder containing a single `report.md`.

---

## Repository: Bench_GitHub_MCP2

```
Bench_GitHub_MCP2/
├── README.md
├── agents/
│   ├── Report.md
│   ├── test_1.md … test_64.md          (flat files, sequential)
│   ├── test_65.md
│   ├── test_65/report.md               (dir)
│   ├── test_66.md … test_73.md
│   ├── test_74.md
│   ├── test_74/report.md               (dir)
│   ├── test_75.md … test_80.md
│   ├── test_81/report.md               (dir)
│   ├── test_82/report.md               (dir)
│   ├── test_83/report.md               (dir)
│   ├── test_84/                        (dir, multi-file)
│   │   ├── commits_part1.md
│   │   ├── commits_part2.md
│   │   ├── commits_part3.md
│   │   ├── commits_part4.md
│   │   ├── commits_part5.md
│   │   └── report.md
│   ├── test_85/report.md               (dir)
│   ├── test_86/report.md               (dir)
│   ├── test_87.md
│   ├── test_87/report.md               (dir)
│   ├── test_88.md
│   ├── test_88/report.md               (dir)
│   ├── test_89/report.md               (dir)
│   ├── test_90.md
│   ├── test_90_part1.md
│   ├── test_90_part2.md
│   ├── test_90/report.md               (dir)
│   ├── test_91.md … test_93.md
│   ├── test_94.md
│   ├── test_94_part01.md … test_94_part10.md
│   ├── test_95.md … test_98.md
│   ├── test_99.md
│   ├── test_99_part01.md … test_99_part10.md
│   ├── test_100.md
│   ├── test_101/report.md              (dir)
│   ├── test_102.md
│   ├── test_102/report.md              (dir)
│   ├── test_102_part01.md … test_102_part10.md
│   ├── test_103.md … test_109.md
│   ├── test_110.md
│   ├── test_110_part01.md … test_110_part10.md
│   ├── test_111.md … test_113.md
│   ├── test_114.md
│   └── test_114_part01.md … test_114_part10.md
└── docs/
    ├── mcp-Key-Concepts.md
    ├── mcp-best-practices-resources.md
    ├── mcp-best-practices.md
    ├── mcp-how-to-code-an-mcp-server.md
    ├── mcp-introduction.md
    ├── mcp-overview.md
    └── mcp-resources.md
```

**Summary:** Root contains `README.md`, an `agents/` folder (114 numbered test entries, several with large "part" files or nested `report.md` subfolders), and a `docs/` folder with 7 MCP-related markdown guides.

---

## Comparison Notes
- Both repos share the same `agents/test_N` convention (flat `.md` file OR a subfolder containing `report.md`).
- `Bench_GitHub_MCP2` is considerably larger (114 test entries vs. 66) and additionally includes a `docs/` folder that `Bench_GitHub_MCP` lacks.
- `Bench_GitHub_MCP2/agents/test_84` is the only folder with multiple content files (5 `commits_part*.md` files plus a `report.md`), whereas all other subfolders in both repos contain exactly one `report.md`.
