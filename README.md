# REST API Patterns Guide

Date: 2026-03-12

## Summary of REST API Best Practices (2024)

- Follow Google's **API Design Guide**: resource‑oriented design, consistent naming, and standard HTTP methods (GET, LIST, CREATE, UPDATE, DELETE).
- Use **resource names** that are stable and hierarchical (e.g., `projects/{project}/databases/{database}`).
- Adopt **standard methods** (AIP‑130 series) for common CRUD operations; custom actions should be clearly named and documented.
- Include **standard fields** such as `name`, `createTime`, `updateTime`, and `etag` for versioning and concurrency control.
- Return **proper HTTP status codes** and provide rich error details following AIP‑193.
- Implement **pagination**, **filtering**, and **ordering** for list endpoints (AIP‑132).
- Use **JSON schema** with clear field types, required properties, and examples.
- Document **versioning** strategy (URI versioning or media type versioning) and maintain backward compatibility (AIP‑185, AIP‑180).
- Apply **security best practices**: OAuth 2.0, JWT, and proper scopes; avoid exposing secrets.
- Follow **design patterns** such as idempotent `PUT`/`PATCH`, use of `ETag` for optimistic locking, and consistent error handling.

Research conducted on 2026-03-12.
