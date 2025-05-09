# 🕸️ Day-35: Java Data Structures – Graphs

Welcome to **Day-35** of our Backend Engineering journey! Today we're exploring **Graphs** — a powerful, flexible data structure that models real-world connections like social networks, web links, and transport maps.

This lesson includes **real-world applications**, a **step-by-step Maven project**, interactive **visuals**, and **JUnit 5 tests** to reinforce your understanding.

---

## 📚 What You'll Learn

- ✅ What is a Graph?
- ✅ Real-world use cases (Why we use them)
- ✅ Representing graphs in Java (adjacency list, edge list)
- ✅ BFS (Breadth-First Search) for connection checking
- ✅ Graph implementation using HashMaps and Lists
- ✅ Testing your graph logic using JUnit 5
- ✅ Maven project structure and OOP best practices

---

## 💬 Summary of Key Concepts

### 🧠 What is a Graph?

A **Graph** is a collection of **nodes (vertices)** and **edges**. It can be:

- **Undirected** (like friendships)
- **Directed** (like Twitter follows)
- **Weighted** (like distances between cities)

### ❓ Why Graphs?

Graphs are essential to model:
- Social networks (Facebook friends)
- Web pages (links between them)
- Pathfinding (Google Maps)
- Recommendation engines (Netflix, YouTube)

### 🛠️ How Graphs Work in Java

We simulate graphs using:

```java
Map<String, List<String>> graph = new HashMap<>();
````

* Add users as **keys**.
* Add friends as **values** in the list.
* Use **BFS** to check if two users are connected.

---

## 🖼️ Visual Aids

### 🌐 A Simple Graph Representation

Imagine a small social network:

```
Alice -- Bob -- Charlie
```

This becomes:

```java
Alice → [Bob]
Bob → [Alice, Charlie]
Charlie → [Bob]
```

### 🔁 Breadth-First Search (BFS)

BFS explores layer by layer. For a connection check:

```
Start: Alice
Visit: Bob
Visit: Charlie → Found!
```
---

### 🌐 Graph Representation in Java

A simple undirected graph can be represented using an adjacency list in Java. Here's a visual example:

![Graph Representation](https://cdn.programiz.com/sites/tutorial2program/files/graph-implementation.png)

---

### 🔁 Breadth-First Search (BFS) Traversal

BFS explores nodes level by level, starting from a selected node and visiting all its neighbors before moving to the next layer.

![BFS Traversal](https://i.giphy.com/media/iD6qdVmNOZH9frN6J4/giphy.gif)

---

### 🧭 Graph Visualization Using Java Libraries

For more complex graphs, you can visualize nodes and edges using Java visualization tools like GraphStream or JUNG:

![Graph Visualization](https://cambridge-intelligence.com/wp-content/uploads/2019/12/spring-keylines-compressor.png)

---

### 🧠 Summary Table: Graph Concepts

| Concept               | Description                                                                 |
|-----------------------|-----------------------------------------------------------------------------|
| **Vertex (Node)**     | Represents an entity in a graph                                             |
| **Edge**              | A connection between two nodes                                              |
| **Adjacency List**    | A map storing each node and its neighbors                                  |
| **BFS Traversal**     | A graph traversal algorithm using a queue                                  |
| **Visualization**     | Diagrams that help explore the graph visually                              |

---

## 🚀 Assignment: FriendNet – A Social Network Simulator 🧑‍🤝‍🧑

You will build a mini-social network where:

* Users can be added.
* Friendships can be created (undirected edges).
* You can check if two users are connected via friends.
* Traversal is done using BFS.

✅ The project uses:

* Java 17+
* Maven
* JUnit 5 for testing
* Clean OOP practices

---

## 🛠️ Project Setup Instructions

### 📦 Maven Setup

If you're creating it manually:

1. Open IntelliJ → New Project → Maven
2. Use:

```text
GroupId: com.friendnet
ArtifactId: friendnet-graph
```

3. Add JUnit 5 in `pom.xml`:

```xml
<dependency>
  <groupId>org.junit.jupiter</groupId>
  <artifactId>junit-jupiter</artifactId>
  <version>5.9.1</version>
  <scope>test</scope>
</dependency>
```

---

## 🔍 File Structure (Suggestion)

```
friendnet-graph/
├── main/
│   └── java/com/friendnet/
│       ├── FriendGraph.java       # Graph logic
│       └── Main.java              # Sample runner
└── test/
    └── java/com/friendnet/
        └── FriendGraphTest.java   # Unit tests
```

---

## 🧪 Testing Guide

Write **JUnit 5 tests** for:

| Class         | Test Class Name   |
| ------------- | ----------------- |
| `FriendGraph` | `FriendGraphTest` |

✅ Use:

* `@BeforeEach`
* `@Test`
* `assertTrue`, `assertFalse`
* `@DisplayName` for clarity

---

## 🧠 Your Tasks

| Task                      | Status |
| ------------------------- | ------ |
| Understand graph concepts | ✅      |
| Clone or fork the repo    | ⏳      |
| Add users & friendships   | ⏳      |
| Implement BFS search      | ⏳      |
| Write and run tests       | ⏳      |
| Push code to GitHub       | ⏳      |
| Submit repo in Slack      | ⏳      |

---

## 📼 Zoom Recording

🎥 **Lecture Recording for Day-35**:
🔗 [Click to Watch](_Will be added later_)

🧪 **Demo Code Exercise**:
[`FriendNet Graph Simulator`](https://github.com/FW-Zalando-Java-Backend-Engineer/FriendNet)

---

## ✍️ Exercise Submission

* Fork the repo and complete the tasks
* Add your name in the `README.md`
* Push changes to GitHub
* 🐙 Submit the link via Slack DM

---

## 🏁 Completion Checklist

* [ ] `FriendGraph` with addUser, addFriendship, getFriends
* [ ] BFS method for checking connection
* [ ] Clean and readable Java code
* [ ] Full test coverage with JUnit 5
* [ ] JavaDocs and inline comments
* [ ] README completed and committed

---

## 📚 References

### 🔹 Medium Articles

* [Graphs in Java – Medium](https://medium.com/@aqibbutt3078/graphs-in-java-94691259710f)
* [Beginner’s Guide to Graph Theory – Medium](https://medium.com/@agarwaldevesh.08/introduction-to-graph-theory-for-beginners-ae33e754dc5e)

### 🔹 Docs & Tools

* [JGraphT Graph Library](https://jgrapht.org/)
* [Java Collections API (Oracle)](https://docs.oracle.com/javase/8/docs/api/java/util/Map.html)




## 🧠 Final Thoughts

> "Graphs are everywhere — from your friend circle to your Spotify recommendations.
> If you can BFS through a network, you can BFS through life!" 😄

Keep coding and stay connected!


