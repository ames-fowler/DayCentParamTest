# Crop Parameter Commons
Governance, Review, and Visibility Policy (v1)

# Purpose
The Crop Parameter Commons provides an open, transparent, and review-gated mechanism for sharing, evaluating, and adopting crop parameterizations used in ecosystem models (e.g., DayCent). The goal is to enable community contribution while maintaining scientific quality, reproducibility, and clear provenance.

This document defines how submissions are reviewed, when they become publicly visible, and how parameterizations are accepted into the shared default library.

# Roles

## Contributors
Contributors submit new crop parameterizations and required metadata, respond to reviewer feedback, and retain authorship and attribution for their submissions.

## Reviewers
Reviewers evaluate submissions against review criteria, approve or request revisions at each review stage, and document decisions and rationale.

## Administrators
Administrators manage review assignments and escalation, approve final acceptance into the default library, and maintain schemas, benchmarks, and system configuration.

# Submission Lifecycle Overview

All submissions progress through a staged review process. Each stage must be completed successfully before advancing.

Review stages are:

- Review-1: Metadata and File Validation

- Review-2: Benchmarking and Performance Checks

- Review-3: Peer-Reviewed Evidence Verification

- Review-4: Acceptance into Default Library

Submissions may be returned for revision or rejected at any stage.

# Visibility Policy

Default (Private)
Newly submitted parameterizations are private by default. They are visible only to the submitter, assigned reviewers, and administrators.

Public After Review-1
After passing Review-1 (Metadata and File Validation), submissions become publicly visible as provisional records. Public visibility includes crop code and version tag, structured metadata, provenance and attribution, and the parameter file (crop.100) or a stable download reference.

This early visibility supports transparency, community feedback, and reuse while clearly signaling provisional status.

# Default Library
Only submissions that pass Review-4 and are explicitly accepted by an administrator are eligible to be designated as defaults and appear in the canonical default parameter library.

# Review Stage Definitions

## Review-1: Metadata and File Validation
Purpose: Ensure submissions are complete, interpretable, and reproducible.

Automated checks may include validation of required metadata fields, metadata schema validation, successful parsing of the parameter file, and computation of content hashes to identify duplicates.

Outcomes include pass (submission becomes public and advances), needs revision (submitter must address issues), or reject (submission does not meet minimum requirements).

## Review-2: Benchmarking and Performance Checks
Purpose: Evaluate model behavior and basic performance.

Typical checks may include generation of development-site schedule files, model runs using standard test harnesses, and evaluation of metrics such as above-ground biomass RMSE by crop and year.

Outputs include benchmark summary metrics, which may be public, and raw benchmark artifacts, which may remain private.

Outcomes include pass, needs revision, or reject.

## Review-3: Peer-Reviewed Evidence Verification
Purpose: Confirm scientific grounding and external validation.

Requirements may include peer-reviewed publications, reports, or datasets; DOI or stable citation references; and reviewer assessment of relevance and applicability.

Outcomes include pass, needs revision, or reject.

## Review-4: Acceptance into Default Library
Purpose: Curate a trusted set of default parameterizations.

Criteria include successful completion of prior review stages, relevance and general applicability, and reviewer and administrator approval.

Outcomes include accepted (eligible to become a default parameterization) or rejected. Only one default parameterization may be designated per crop code at a time.

# Status Labels and Workflow

The review process is tracked using the following GitHub labels:
- review-1
- review-2
- review-3
- review-4
- needs-revision
- rejected
- accepted-default

Labels communicate review state to both humans and automated workflows.

# Attribution and Licensing

Contributors retain authorship and attribution for submitted parameterizations. All submissions must include a clear license permitting reuse. Provenance metadata is preserved permanently.

# Transparency and Auditability

Review decisions, status changes, and timestamps are recorded. Public records clearly indicate provisional versus default status. Historical versions remain accessible for reproducibility.

# Versioning and Updates

Accepted parameterizations are immutable. Updates require submission of a new version. This governance document may evolve; changes will be versioned and documented.

# Guiding Principle

Early transparency, staged rigor, and explicit provenance.
Submissions are shared openly once minimally validated, while defaults are curated through deliberate, evidence-based review.
