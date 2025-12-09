# Tasks: AI/Spec-Driven Book on Physical AI & Humanoid Robotics

**Input**: Design documents from `/specs/AI-Spec-Driven-Book-on-Physical-AI-Humanoid-Robotics/`
**Prerequisites**: plan.md (required), spec.md (required for user stories), research.md, data-model.md, contracts/

**Tests**: The examples below include test tasks. Tests are OPTIONAL - only include them if explicitly requested in the feature specification.

**Organization**: Tasks are grouped by user story to enable independent implementation and testing of each story.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2, US3)
- Include exact file paths in descriptions

## Path Conventions

- **Single project**: `src/`, `tests/` at repository root
- **Web app**: `backend/src/`, `frontend/src/`
- **Mobile**: `api/src/`, `ios/src/` or `android/src/`
- Paths shown below assume Docusaurus-centric structure - adjust based on plan.md structure

## Phase 1: Setup (Project Initialization & Docusaurus Foundation)

**Purpose**: Establish the core Docusaurus project and repository structure.

- [ ] T001 Initialize Docusaurus project in `book-repo/`
- [ ] T002 Create `docs/` and `static/` directories in `book-repo/`
- [ ] T003 Configure `docusaurus.config.js` for basic site metadata in `book-repo/docusaurus.config.js`
- [ ] T004 Create `sidebars.js` for initial documentation hierarchy in `book-repo/sidebars.js`
- [ ] T005 Create `code-examples/` root directory in `book-repo/code-examples/`
- [ ] T006 Add Docusaurus-specific dependencies to `book-repo/package.json`
- [ ] T007 Initialize git repository and add `.gitignore` for common Docusaurus files in `book-repo/.gitignore`

---

## Phase 2: Foundational (Research & Scaffolding)

**Purpose**: Conduct initial research and define chapter scaffolds based on the plan.

**⚠️ CRITICAL**: No user story work can begin until this phase is complete.

### Research for Core Concepts
- [ ] T008 Collect authoritative robotics sources (ROS 2 REP docs, Isaac papers, Gazebo manuals, peer-reviewed papers) in `research.md`
- [ ] T009 Extract validated concepts for Physical AI and embodied intelligence for `research.md`
- [ ] T010 Extract validated concepts for humanoid robotics for `research.md`

### Chapter Scaffolding
- [ ] T011 Define chapter scaffolds using Spec-Kit Plus for ROS 2 content in `docs/ros2/`
- [ ] T012 Define chapter scaffolds using Spec-Kit Plus for Gazebo content in `docs/gazebo/`
- [ ] T013 Define chapter scaffolds using Spec-Kit Plus for Unity content in `docs/unity/`
- [ ] T014 Define chapter scaffolds using Spec-Kit Plus for NVIDIA Isaac content in `docs/nvidia-isaac/`
- [ ] T015 Define chapter scaffolds using Spec-Kit Plus for VLA robotics content in `docs/vla-robotics/`

**Checkpoint**: Foundation ready - user story implementation can now begin in parallel.

---

## Phase 3: User Story 1 - Learning Core Concepts and Reproducible Examples (Priority: P1) 🎯 MVP

**Goal**: Students understand core concepts and can reproduce examples across ROS 2, Gazebo, Unity, and Isaac Sim.

**Independent Test**: Student can follow any chapter tutorial, execute its provided code/simulation, and achieve the described outcome without external assistance, demonstrating successful learning and reproducibility.

### Implementation for User Story 1 (ROS 2 Focus)
- [ ] T016 [US1] Draft chapter content for ROS 2 core concepts in `docs/ros2/chapter-1.md`
- [ ] T017 [US1] Create a basic reproducible ROS 2 example in `code-examples/ros2-examples/basic-publisher-subscriber/`
- [ ] T018 [US1] Integrate ROS 2 example into `docs/ros2/chapter-1.md`
- [ ] T019 [US1] Verify ROS 2 example reproducibility on target environment
- [ ] T020 [US1] Perform citation audit for ROS 2 chapter content for APA format compliance in `docs/ros2/chapter-1.md`
- [ ] T021 [US1] Run plagiarism scan for `docs/ros2/chapter-1.md`

### Implementation for User Story 1 (Gazebo Focus)
- [ ] T022 [P] [US1] Draft chapter content for Gazebo simulation basics in `docs/gazebo/chapter-1.md`
- [ ] T023 [P] [US1] Create a basic reproducible Gazebo simulation in `code-examples/gazebo-simulations/simple-robot/`
- [ ] T024 [P] [US1] Integrate Gazebo simulation into `docs/gazebo/chapter-1.md`
- [ ] T025 [P] [US1] Verify Gazebo simulation reproducibility on target environment
- [ ] T026 [P] [US1] Perform citation audit for Gazebo chapter content for APA format compliance in `docs/gazebo/chapter-1.md`
- [ ] T027 [P] [US1] Run plagiarism scan for `docs/gazebo/chapter-1.md`

### Implementation for User Story 1 (Unity Focus)
- [ ] T028 [P] [US1] Draft chapter content for Unity for robotics introduction in `docs/unity/chapter-1.md`
- [ ] T029 [P] [US1] Create a basic reproducible Unity robot project in `code-examples/unity-projects/basic-robot-arm/`
- [ ] T030 [P] [US1] Integrate Unity project into `docs/unity/chapter-1.md`
- [ ] T031 [P] [US1] Verify Unity project reproducibility on target environment
- [ ] T032 [P] [US1] Perform citation audit for Unity chapter content for APA format compliance in `docs/unity/chapter-1.md`
- [ ] T033 [P] [US1] Run plagiarism scan for `docs/unity/chapter-1.md`

### Implementation for User Story 1 (NVIDIA Isaac Focus)
- [ ] T034 [P] [US1] Draft chapter content for NVIDIA Isaac Sim introduction in `docs/nvidia-isaac/chapter-1.md`
- [ ] T035 [P] [US1] Create a basic reproducible NVIDIA Isaac Sim asset/example in `code-examples/nvidia-isaac-assets/simple-scene/`
- [ ] T036 [P] [US1] Integrate NVIDIA Isaac Sim example into `docs/nvidia-isaac/chapter-1.md`
- [ ] T037 [P] [US1] Verify NVIDIA Isaac Sim example reproducibility on target environment
- [ ] T038 [P] [US1] Perform citation audit for NVIDIA Isaac chapter content for APA format compliance in `docs/nvidia-isaac/chapter-1.md`
- [ ] T039 [P] [US1] Run plagiarism scan for `docs/nvidia-isaac/chapter-1.md`

**Checkpoint**: User Story 1 should be fully functional and testable independently across all core platforms.

---

## Phase 4: User Story 2 - Transitioning to Physical Robot Systems (Priority: P1)

**Goal**: Engineers learn about Physical AI systems integrating ROS 2, Gazebo, Unity, and NVIDIA Isaac, including an end-to-end vision-language-action pipeline using Whisper + LLMs.

**Independent Test**: Engineer can successfully implement and demonstrate the full LLM-to-ROS action translation pipeline, taking voice input and translating it to cognitive planning and robot action within a simulated environment.

### Implementation for User Story 2 (Integration & VLA Pipeline)
- [ ] T040 [US2] Draft chapter content on integrating ROS 2, Gazebo, Unity, and NVIDIA Isaac in `docs/vla-robotics/chapter-1.md`
- [ ] T041 [US2] Develop the Whisper + LLM component for voice input processing in `code-examples/vla-pipeline-code/whisper-llm-processor.py`
- [ ] T042 [US2] Develop the cognitive planning component (LLM output to ROS actions) in `code-examples/vla-pipeline-code/cognitive-planner.py`
- [ ] T043 [US2] Create a ROS 2 action server for robot actions in `code-examples/ros2-examples/robot-action-server/`
- [ ] T044 [US2] Integrate Whisper, LLM, cognitive planner, and ROS 2 action server for end-to-end pipeline in `code-examples/vla-pipeline-code/full-pipeline.py`
- [ ] T045 [US2] Create a reproducible simulation environment for the VLA pipeline in `code-examples/gazebo-simulations/vla-robot-scenario/` or `code-examples/nvidia-isaac-assets/vla-robot-scene/`
- [ ] T046 [US2] Integrate VLA pipeline example into `docs/vla-robotics/chapter-1.md`
- [ ] T047 [US2] Verify end-to-end VLA pipeline functionality with voice input to robot action
- [ ] T048 [US2] Perform citation audit for VLA robotics chapter content for APA format compliance in `docs/vla-robotics/chapter-1.md`
- [ ] T049 [US2] Run plagiarism scan for `docs/vla-robotics/chapter-1.md`

**Checkpoint**: User Stories 1 AND 2 should both work independently.

---

## Phase 5: User Story 3 - Building Physical-AI-focused Curricula (Priority: P2)

**Goal**: Educators get a comprehensive resource that clearly explains Physical AI, embodied intelligence, and humanoid robotics, with verifiable citations and a complete Docusaurus website and PDF version.

**Independent Test**: Educator can utilize the book's content, verify its citations, and confirm the Docusaurus/PDF outputs, and then construct a coherent course module directly from the book.

### Implementation for User Story 3 (Curation & Publishing)
- [ ] T050 [P] [US3] Review and refine all chapter content for writing clarity (Flesch-Kincaid grade 10–12) across `docs/`
- [ ] T051 [P] [US3] Consolidate all citation audits and ensure minimum 50% peer-reviewed sources across all `docs/` chapters
- [ ] T052 [P] [US3] Run final plagiarism scan for the entire book content in `docs/`
- [ ] T053 [P] [US3] Configure Docusaurus build process to generate website and PDF output in `book-repo/docusaurus.config.js` and `scripts/`
- [ ] T054 [US3] Build the Docusaurus website and verify no broken links or sidebar inconsistencies (Docusaurus build output)
- [ ] T055 [US3] Generate the PDF version of the book and verify APA citations and formatting (PDF output)
- [ ] T056 [US3] Prepare deployment instructions for chosen publishing platform (e.g., GitHub Pages or Netlify) in `README.md`

**Checkpoint**: All user stories should now be independently functional.

---

## Phase 6: Polish & Cross-Cutting Concerns

**Purpose**: Final improvements and quality checks across the entire book.

- [ ] T057 Update `sidebars.js` for final chapter order and navigation in `book-repo/sidebars.js`
- [ ] T058 Review and integrate all ADRs (Architectural Decision Records) into relevant chapter introductions or dedicated sections
- [ ] T059 Review all code-examples for consistency and clarity
- [ ] T060 Update README.md with project overview, setup instructions, and deployment guide in `book-repo/README.md`
- [ ] T061 Final review of the entire Docusaurus site for user experience and content flow
- [ ] T062 Generate final PDF version and review for print readiness

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: Depends on Setup completion - BLOCKS all user stories
- **User Stories (Phase 3+)**: All depend on Foundational phase completion
  - User stories can then proceed in parallel (if staffed)
  - Or sequentially in priority order (P1 → P2 → P3)
- **Polish (Final Phase)**: Depends on all desired user stories being complete

### User Story Dependencies

- **User Story 1 (P1)**: Can start after Foundational (Phase 2) - No dependencies on other stories
- **User Story 2 (P1)**: Can start after Foundational (Phase 2) - May integrate with US1 components (e.g., existing simulation setups) but should be independently testable for its core VLA functionality.
- **User Story 3 (P2)**: Can start after Foundational (Phase 2) - Depends on content creation and example integration from US1 and US2 for its validation tasks.

### Within Each User Story

- Content drafting before example integration.
- Example creation before reproducibility verification.
- Verification, citation audit, and plagiarism scans after content and examples are stable.

### Parallel Opportunities

- All Setup tasks (T001-T007) can run in parallel.
- Chapter scaffolding tasks (T011-T015) can run in parallel within Foundational Phase.
- Within User Story 1, tasks for different platforms (ROS 2, Gazebo, Unity, NVIDIA Isaac) can run in parallel (e.g., T016-T021 parallel with T022-T027, etc.).
- Once Foundational phase completes, User Story 1 and User Story 2 (P1) can ideally start in parallel. User Story 3 (P2) can start when US1 and US2 content is sufficiently developed for review and publishing tasks.

---

## Parallel Example: User Story 1 (ROS 2, Gazebo, Unity, NVIDIA Isaac)

```bash
# Launch drafting and example creation for all platforms in parallel:
Task: "Draft chapter content for ROS 2 core concepts in docs/ros2/chapter-1.md"
Task: "Create a basic reproducible ROS 2 example in code-examples/ros2-examples/basic-publisher-subscriber/"

Task: "Draft chapter content for Gazebo simulation basics in docs/gazebo/chapter-1.md"
Task: "Create a basic reproducible Gazebo simulation in code-examples/gazebo-simulations/simple-robot/"

Task: "Draft chapter content for Unity for robotics introduction in docs/unity/chapter-1.md"
Task: "Create a basic reproducible Unity robot project in code-examples/unity-projects/basic-robot-arm/"

Task: "Draft chapter content for NVIDIA Isaac Sim introduction in docs/nvidia-isaac/chapter-1.md"
Task: "Create a basic reproducible NVIDIA Isaac Sim asset/example in code-examples/nvidia-isaac-assets/simple-scene/"
```

---

## Implementation Strategy

### MVP First (User Story 1 Focus)

1.  Complete Phase 1: Setup
2.  Complete Phase 2: Foundational (CRITICAL - blocks all stories)
3.  Complete Phase 3: User Story 1 (focus on getting all core platform examples and content stable).
4.  **STOP and VALIDATE**: Test User Story 1 independently across all platforms.
5.  Deploy/demo initial Docusaurus site with US1 content.

### Incremental Delivery

1.  Complete Setup + Foundational → Foundation ready.
2.  Complete User Story 1 → Test independently → Deploy/Demo (MVP with core platform examples).
3.  Complete User Story 2 → Test independently → Deploy/Demo (Add VLA pipeline).
4.  Complete User Story 3 → Test independently → Deploy/Demo (Finalized book, Docusaurus, PDF).
5.  Each story adds value without breaking previous stories.

### Parallel Team Strategy

With multiple developers:

1.  Team completes Setup + Foundational together.
2.  Once Foundational is done:
    *   Developer A: User Story 1 (focus on ROS 2 and Gazebo content/examples).
    *   Developer B: User Story 1 (focus on Unity and NVIDIA Isaac content/examples).
    *   Developer C: User Story 2 (VLA pipeline development).
    *   Developer D: User Story 3 (Curriculum and publishing pipeline, once sufficient content is available).
3.  Stories complete and integrate independently.

---

## Notes

- [P] tasks = different files, no dependencies
- [Story] label maps task to specific user story for traceability
- Each user story should be independently completable and testable
- Verify tests fail before implementing
- Commit after each task or logical group
- Stop at any checkpoint to validate story independently
- Avoid: vague tasks, same file conflicts, cross-story dependencies that break independence
