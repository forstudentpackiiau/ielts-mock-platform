ielts-mock-platform/
│
├── app/
│   ├── layout.tsx                 # Root layout (auth + role guard)
│   ├── page.tsx                   # Landing / login redirect
│   ├── globals.css
│   │
│   ├── auth/
│   │   └── login/
│   │       └── page.tsx           # Login page
│   │
│   ├── super-admin/
│   │   ├── layout.tsx             # SUPER_ADMIN sidebar
│   │   ├── dashboard/
│   │   │   └── page.tsx
│   │   ├── centers/
│   │   │   └── page.tsx
│   │   └── reports/
│   │       └── page.tsx
│   │
│   ├── center-admin/
│   │   ├── layout.tsx
│   │   ├── dashboard/
│   │   │   └── page.tsx
│   │   ├── classes/
│   │   │   └── page.tsx
│   │   ├── teachers/
│   │   │   └── page.tsx
│   │   ├── students/
│   │   │   └── page.tsx
│   │   └── assign-tests/
│   │       └── page.tsx
│   │
│   ├── teacher/
│   │   ├── layout.tsx
│   │   ├── dashboard/
│   │   │   └── page.tsx
│   │   ├── mock-tests/
│   │   │   ├── page.tsx
│   │   │   ├── create/
│   │   │   │   └── page.tsx
│   │   │   └── edit/
│   │   │       └── [testId]/
│   │   │           ├── page.tsx
│   │   │           ├── publish/
│   │   │           │   └── page.tsx
│   │   │           └── section/
│   │   │               └── [sectionId]/
│   │   │                   └── questions/
│   │   │                       └── page.tsx
│   │   ├── submissions/
│   │   │   └── page.tsx
│   │   └── analytics/
│   │       └── page.tsx
│   │
│   ├── student/
│   │   ├── layout.tsx
│   │   ├── dashboard/
│   │   │   └── page.tsx
│   │   ├── assigned-tests/
│   │   │   └── page.tsx
│   │   ├── take-test/
│   │   │   └── [assignmentId]/
│   │   │       └── page.tsx
│   │   └── results/
│   │       └── [submissionId]/
│   │           └── page.tsx
│   │
│   └── api/
│       ├── auth/
│       │   └── [...nextauth]/
│       │       └── route.ts
│       │
│       ├── mock-tests/
│       │   ├── route.ts
│       │   └── [testId]/
│       │       ├── route.ts
│       │       ├── publish/
│       │       │   └── route.ts
│       │       └── sections/
│       │           ├── route.ts
│       │           └── [sectionId]/
│       │               └── questions/
│       │                   └── route.ts
│       │
│       ├── assignments/
│       │   └── route.ts
│       │
│       ├── student/
│       │   ├── assigned-tests/
│       │   │   └── route.ts
│       │   ├── start-test/
│       │   │   └── route.ts
│       │   ├── save-answer/
│       │   │   └── route.ts
│       │   ├── submit-test/
│       │   │   └── route.ts
│       │   └── submissions/
│       │       └── route.ts
│       │
│       ├── ai/
│       │   ├── evaluate/
│       │   │   └── route.ts
│       │   ├── scores/
│       │   │   └── route.ts
│       │   └── override/
│       │       └── route.ts
│       │
│       └── dashboards/
│           ├── super-admin/
│           │   └── route.ts
│           ├── center-admin/
│           │   └── route.ts
│           └── teacher/
│               └── route.ts
│
├── components/
│   ├── ui/                        # shadcn/ui components
│   │   ├── button.tsx
│   │   ├── card.tsx
│   │   ├── input.tsx
│   │   ├── table.tsx
│   │   ├── modal.tsx
│   │   └── select.tsx
│   │
│   ├── layout/
│   │   ├── Sidebar.tsx
│   │   ├── Topbar.tsx
│   │   └── RoleGuard.tsx
│   │
│   ├── forms/
│   │   ├── MockTestForm.tsx
│   │   ├── SectionForm.tsx
│   │   ├── QuestionForm.tsx
│   │   └── OverrideScoreForm.tsx
│   │
│   ├── charts/
│   │   ├── AverageScoreChart.tsx
│   │   └── WeakAreasChart.tsx
│   │
│   └── tables/
│       ├── StudentsTable.tsx
│       ├── SubmissionsTable.tsx
│       └── MockTestsTable.tsx
│
├── lib/
│   ├── prisma.ts                  # Prisma client
│   ├── auth.ts                    # Role-based auth helpers
│   ├── permissions.ts             # RBAC rules
│   ├── validators.ts              # Zod schemas
│   ├── ai.ts                      # AI prompt + client
│   └── utils.ts
│
├── prisma/
│   ├── schema.prisma
│   └── migrations/
│
├── public/
│   └── logo.svg
│
├── .env
├── .env.example
├── next.config.js
├── tailwind.config.js
├── tsconfig.json
├── package.json
└── README.md
