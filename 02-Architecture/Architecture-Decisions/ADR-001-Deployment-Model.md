# ADR-001: Deployment Model

**Status:** Accepted

**Date:** July 2026

---

# Context

The project requires a secure and maintainable deployment model for hosting Nextcloud in an enterprise environment.

The solution must:

- Protect sensitive business data.
- Support secure remote access.
- Allow future scalability.
- Follow security best practices.
- Be suitable for a small to medium-sized organisation.

Several deployment approaches were considered before selecting the final architecture.

---

# Options Considered

## Option 1 – Single Server Deployment

All components (web server, application, and database) are installed on a single Ubuntu server.

### Advantages

- Simple deployment
- Low infrastructure cost
- Easy administration
- Suitable for development and small environments

### Disadvantages

- Single point of failure
- Limited scalability
- Shared resources between application and database
- Less network isolation

---

## Option 2 – Three-Tier Architecture (Selected)

Separate logical layers are used for:

- Client Layer
- Application Layer
- Database Layer

### Advantages

- Better separation of responsibilities
- Easier security control implementation
- Supports future scaling
- Better aligns with enterprise architecture principles
- Reduced attack surface between components

### Disadvantages

- Slightly more complex architecture
- Additional administration effort

---

## Option 3 – Cloud SaaS Storage

Use a third-party cloud storage provider instead of self-hosting.

### Advantages

- Minimal infrastructure management
- High availability
- Vendor-managed updates

### Disadvantages

- Reduced control over business data
- Dependency on external providers
- Less flexibility for security architecture demonstrations

---

# Decision

The project adopts a **three-tier deployment model** consisting of:

- Client Layer
- Application Layer
- Database Layer

Although the implementation is performed within a single virtual machine for demonstration purposes, the architecture is designed as if each layer could be deployed independently in a production environment.

This approach provides a balance between practical implementation and enterprise architectural design.

---

# Security Considerations

The selected deployment model supports:

- Defence in depth
- Principle of least privilege
- Secure communication using HTTPS
- Network segmentation
- Layered security controls
- Future high availability options

---

# Consequences

### Positive

- Easier application of security controls
- Clear trust boundaries
- Better scalability
- Simplified future migration
- Better alignment with enterprise security architecture practices

### Negative

- Additional design complexity
- More documentation required
- Higher operational overhead in large deployments

---

# Future Improvements

The architecture can later be extended to include:

- Reverse proxy load balancing
- Multiple Nextcloud application servers
- PostgreSQL replication
- Object storage
- Centralised logging and monitoring
- SIEM integration
- High availability clustering

---

# Related Documents

- Business Requirements
- Security Objectives
- Deployment Model
- Security Requirements
- Trust Boundaries
- STRIDE Analysis
- Risk Assessment