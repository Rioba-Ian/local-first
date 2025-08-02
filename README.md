# Local-First Development Examples

This repository contains multiple example projects showcasing different approaches to building **local-first applications**. Local-first software gives users agency over their data while providing fast, responsive user experiences that work offline and sync seamlessly across devices.

## What is Local-First?

Local-first applications prioritize:

- **Fast performance** - Data is stored locally for instant interactions
- **Offline capabilities** - Apps work without network connectivity
- **Data ownership** - Users control their data
- **Real-time collaboration** - Changes sync automatically across devices
- **Resilience** - No single point of failure

## Projects Overview

### 🚀 [Zero (Rocicorp) Examples](./hello-zero/)

**Tech Stack:** Zero, React, PostgreSQL, TypeScript

Zero provides a complete local-first stack with real-time sync and conflict resolution.

**Key Features:**

- Declarative client-side schema with relationships
- Built-in permissions system with fine-grained access control
- Real-time multiplayer capabilities
- Optimistic updates with automatic rollback
- PostgreSQL integration with WAL-based replication

**Use Cases:**

- Real-time chat applications
- Collaborative document editing
- Multi-user dashboards
- Social media platforms

---

### ⚡ [TanStack DB + Electric SQL](./my-tanstack-db-project/)

**Tech Stack:** TanStack Start, TanStack DB, Electric SQL, tRPC, Drizzle ORM, PostgreSQL

A full-stack starter combining TanStack's client-side database with Electric SQL's sync engine.

**Key Features:**

- Sub-millisecond live queries with joins and aggregates
- Differential dataflow query engine
- Type-safe mutations via tRPC
- Real-time sync with Electric SQL shapes
- Authentication with better-auth
- Local HTTPS development with Caddy

**Use Cases:**

- Project management tools
- Task tracking applications
- Collaborative workspaces
- Data-heavy dashboards

---

### 📦 [TinyBase Examples](./my-tinybase-app/)

**Tech Stack:** TinyBase, React, TypeScript, Vite

TinyBase offers a lightweight, reactive data store for building local-first apps.

**Key Features:**

- Tiny footprint (~10KB gzipped)
- Reactive data store with relationships
- Built-in UI components for React
- Flexible schema with tables, indexes, and metrics
- Persistence adapters for various storage backends

**Use Cases:**

- Small to medium-sized apps
- Mobile applications
- Embedded systems
- Prototyping and experimentation

---

### 🔄 [Convex Integration](./lofi-zero/convex/)

**Tech Stack:** Convex, React, TypeScript

Exploring local-first patterns with Convex's backend-as-a-service platform. It is more of a BaaS solution that provides serverless functions and real-time data sync. Their approach is not exactly local-first but can be adapted for local-first patterns.

**Key Features:**

- Server-side functions with automatic client sync
- Real-time subscriptions
- Optimistic updates
- Built-in authentication and authorization
- TypeScript-first development experience

**Use Cases:**

- Rapid prototyping
- Apps requiring backend logic
- Real-time collaborative features
- Applications with complex business logic

---

### 🧪 [Legend State Examples](./lofi-zero/legend-state/)

**Tech Stack:** Legend State, React, TypeScript

Legend State provides fine-grained reactivity and persistence for React applications.

**Key Features:**

- Minimal re-renders with fine-grained reactivity
- Automatic persistence to various backends
- Optimistic updates with sync
- Type-safe state management
- Easy integration with existing React apps

**Use Cases:**

- Performance-critical applications
- Complex state management scenarios
- Apps requiring fine-grained reactivity
- Migration from other state management solutions

---

### 🔌 [Electric SQL Examples](./lofi-zero/electric-sql/)

**Tech Stack:** Electric SQL, React, PostgreSQL

Direct integration with Electric SQL for PostgreSQL-based local-first applications.

**Key Features:**

- Postgres-compatible local database (SQLite)
- Bidirectional sync with conflict resolution
- Partial replication with shapes
- Works with existing Postgres databases
- Rich querying capabilities with SQL

**Use Cases:**

- Existing PostgreSQL applications
- Complex relational data models
- Applications requiring SQL queries
- Enterprise data synchronization

## Getting Started

Each project contains its own README with detailed setup instructions. Here's a general approach:

1. **Choose your stack** based on your requirements:

   - **Zero**: Best for real-time multiplayer apps
   - **TanStack DB + Electric**: Best for complex data queries and full-stack TypeScript
   - **TinyBase**: Best for lightweight, simple applications
   - **Convex**: Best for rapid prototyping with backend features
   - **Legend State**: Best for performance-critical React apps
   - **Electric SQL**: Best for existing PostgreSQL applications

2. **Navigate to the project directory**:

   ```bash
   cd [project-name]
   ```

3. **Follow the project-specific README** for installation and setup

## Architecture Patterns

### Data Flow Patterns

- **Optimistic Updates**: Changes applied locally first, then synced
- **Conflict Resolution**: Automatic handling of concurrent edits
- **Real-time Sync**: Live updates across all connected clients
- **Offline Support**: Full functionality without network connectivity

### Common Technologies

- **Frontend**: React, TypeScript, Vite
- **Database**: PostgreSQL, SQLite, IndexedDB
- **Sync**: WebSockets, HTTP streaming, operational transforms
- **Authentication**: JWT, better-auth, custom solutions

## Comparison Matrix

| Feature          | Zero   | TanStack+Electric | TinyBase | Convex | Legend State | Electric SQL |
| ---------------- | ------ | ----------------- | -------- | ------ | ------------ | ------------ |
| Bundle Size      | Medium | Large             | Tiny     | Medium | Small        | Medium       |
| Learning Curve   | Medium | High              | Low      | Medium | Low          | Medium       |
| Real-time Sync   | ✅     | ✅                | ⚠️       | ✅     | ✅           | ✅           |
| Offline Support  | ✅     | ✅                | ✅       | ⚠️     | ✅           | ✅           |
| Complex Queries  | ✅     | ✅                | ⚠️       | ✅     | ⚠️           | ✅           |
| Type Safety      | ✅     | ✅                | ✅       | ✅     | ✅           | ✅           |
| Production Ready | ✅     | 🚧                | ✅       | ✅     | ✅           | 🚧           |

**Legend:**

- ✅ Excellent support
- ⚠️ Limited or requires additional setup
- 🚧 In development/beta

## Contributing

Feel free to add more examples or improve existing ones! Each project should demonstrate:

- Local-first principles
- Real-world use cases
- Best practices and patterns
- Clear documentation

## Resources

### Learning Materials

- [Local-First Software Principles](https://www.inkandswitch.com/local-first/)
- [Zero Documentation](https://zero.rocicorp.dev/)
- [TanStack DB Guide](https://tanstack.com/db/latest)
- [Electric SQL Documentation](https://electric-sql.com/)
- [TinyBase Documentation](https://tinybase.org/)

### Community

- [Local-First Community](https://localfirstweb.dev/)
- [Electric SQL Discord](https://discord.electric-sql.com/)
- [TanStack Discord](https://tlinz.com/discord)

---

_Each example in this repository represents a different approach to building local-first applications. Choose the one that best fits your project requirements and team expertise._
