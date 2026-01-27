# APS145 - Applied Problem Solving (Professional Redesign)

## Course Philosophy

**Original Constraint**: Students must learn pseudocode/flowcharts before touching code  
**Professional Reality**: Problem decomposition is a skill, not a syntax exercise

This redesign maintains all original learning objectives while introducing professional development practices from day one. Students will learn computational thinking through the lens of how actual software is built, not academic exercises.

---

## Course Structure

### The Paradigm Shift

**Instead of**: "Here's pseudocode notation, memorize these symbols"  
**We teach**: "Here's a problem. Let's break it down. Here are multiple valid ways to express solutions."

**Instead of**: Flowcharts as documentation  
**We teach**: Flowcharts as communication tools for stakeholders; pseudocode as architect sketches; diagrams as system design

---

## Weekly Curriculum (Redesigned)

### Week 1: Problem Decomposition & System Thinking
**Original**: Computational Thinking Model  
**Enhanced**: 
- Mental models: How computers vs humans solve problems
- Problem decomposition in the wild (show real GitHub issues → PRs)
- **Intro to version control concepts** (not Git yet, but the *why*)
- **Activity 1**: Same requirements, but students also document:
  - What assumptions did you make?
  - What edge cases exist?
  - How would this scale?

**Deliverable**: Traditional flowchart/pseudocode + "production readiness checklist"

---

### Week 2: Data Representation & State Management
**Original**: Variables, Sequential Logic  
**Enhanced**:
- Variables as state containers
- **Why naming matters**: Code reviews, maintainability, team collaboration
- **Introduction to typing systems** (even in pseudocode - what happens when email is a number?)
- Data validation as first-class concern
- **Activity 2**: Email generator + rainfall analysis
  - Add: Input validation pseudocode
  - Add: Error handling strategy
  - Add: "What would the API contract look like?"

**Connection to Reality**: Show how this maps to JSON schemas, API specs, database schemas

---

### Week 3: Modularity & Interfaces
**Original**: Closed-box functions, Returns  
**Enhanced**:
- Functions as contracts
- **Interface design**: What should be exposed vs hidden?
- **Side effects and purity**: Why it matters
- **Function composition**: Building complex behavior from simple pieces
- **Intro to testing mindset**: How do you verify SendEmail worked?

**Activity 3**: Same requirements, but add:
- Design the "black box" interfaces explicitly
- Document pre/post conditions
- Create test cases in pseudocode

**Real-world parallel**: Introduce concept of API design, microservices boundaries

---

### Week 4: Control Flow & Decision Trees
**Original**: Selection, Nesting  
**Enhanced**:
- Decision trees → state machines (intro)
- **Complexity analysis**: Nested ifs vs lookup tables vs polymorphism
- **Code smells**: When nesting suggests missing abstraction
- Guard clauses and early returns
- **Error handling patterns**

**Activity 4**: Selection problems + 
- Identify code smells in provided pseudocode
- Refactor deeply nested logic
- Document decision rationale

**Professional tie-in**: Configuration management, feature flags, rule engines

---

### Week 5: Iteration & Computational Complexity
**Original**: Loops (mandatory/optional)  
**Enhanced**:
- **Why loops exist**: Humans don't scale, machines do
- Loop invariants (informal)
- **Big O intro** (conceptual, not mathematical)
- When to loop vs when to recurse vs when to vectorize
- **Infinite loops and circuit breakers**

**Activity 5**: Loop problems +
- Estimate time complexity in plain English
- Identify performance bottlenecks
- Propose optimizations

**Real-world connection**: Database query optimization, pagination, rate limiting

---

### Week 6: Collections & Data Structures (Part 1)
**Original**: Introduction to arrays  
**Enhanced**:
- **Why arrays aren't enough**: Introduction to abstract data types
- Array → List → Set → Map mental model
- **When to use which structure**
- Memory implications (conceptual)
- **Activity 6**: Collection problems +
  - Choose appropriate data structure for each problem
  - Justify your choice
  - What are the tradeoffs?

**Professional angle**: Database normalization concepts, caching strategies

---

### Week 7: MIDTERM
- **Modified format**: Part 1 traditional pseudocode/flowcharts (70%)
- **Part 2**: System design scenario (30%)
  - Given a real-world problem, sketch the solution architecture
  - Identify components, data flows, edge cases
  - No single "right" answer - graded on reasoning

---

### Week 8: Advanced Data Modeling
**Original**: Data Structures (simple)  
**Enhanced**:
- **Composition over inheritance** in data design
- **Normalization vs denormalization**
- Structures as domain models
- **Activity 7**: Data structure problems +
  - Design a data model for a real system (e.g., library, e-commerce)
  - Document relationships
  - Identify potential issues

**Professional parallel**: Database design, ORMs, schema migrations

---

### Week 9: Composition & Advanced Abstraction
**Original**: Data Structures (composition)  
**Enhanced**:
- **Separation of concerns**
- **Dependency injection** (conceptual)
- **Builder patterns, factories** (in pseudocode)
- When abstraction helps vs hurts
- **Activity 8**: Refactor poorly designed pseudocode
  - Extract responsibilities
  - Apply SOLID principles (introduce informally)
  - Document design decisions

**Real-world**: Microservices, modular architecture, plugin systems

---

### Week 10: State Machines & Event-Driven Design
**Original**: Timer Logic, State Machines  
**Enhanced**:
- **Event-driven vs procedural thinking**
- State machines as specification tools
- **Asynchronous thinking intro**
- Timer logic → scheduling systems
- **Activity 9**: Design a state machine for:
  - Order fulfillment system
  - Game character behavior
  - Document all states, transitions, guards

**Professional application**: Workflow engines, saga patterns, job queues

---

### Week 11: System Integration & Data Flow
**Original**: Inventory Management Part 1  
**Enhanced**:
- **How systems talk**: APIs, messages, events
- **Data consistency across boundaries**
- Transaction concepts (informal)
- **Activity 10**: Design end-to-end data flow
  - Multiple interconnected systems
  - Error propagation
  - Rollback strategies

**Real-world**: Distributed systems, event sourcing, CQRS (concepts only)

---

### Week 12: Good Friday (College Closed)
**Optional Self-Study Module**: 
- DevOps culture reading
- CI/CD concepts
- Infrastructure as code (what it means)
- **Prepare**: Final presentation outline

---

### Week 13: Synthesis & Presentation
**Original**: Presentation based on Activity 8 or 9  
**Enhanced**:
- **Presentation format**: Act as if pitching to stakeholders
- **Required elements**:
  - Problem statement & constraints
  - Solution architecture (flowcharts/diagrams)
  - Design decisions & tradeoffs
  - **What would break at scale?**
  - **How would you monitor this?**
  - **How would you test this?**

**Grading includes**: Technical correctness + Communication + Systems thinking

---

### Week 14: FINAL EXAM
**Modified format**:
- **Part 1** (50%): Traditional pseudocode/flowchart problems
- **Part 2** (30%): System design & architecture
- **Part 3** (20%): Design critique
  - Given flawed pseudocode/design
  - Identify issues
  - Propose fixes
  - Explain reasoning

---

## Grading Breakdown (Modified)

| Component | Original % | New % | Changes |
|-----------|-----------|-------|---------|
| Activities (1-9) | 25.65% | 25.65% | Same weight, enhanced requirements |
| Activity 10 | - | - | Incorporated into activities |
| Presentation | 10% | 10% | Enhanced criteria |
| Midterm | 35% | 30% | Reduced 5% |
| Final | 35% | 34.35% | Redistributed |
| **NEW: Design Thinking** | - | **+5%** | Added to activities as bonus criteria |

**Total**: 100%

---

## Key Enhancements to Activities

### Every Activity Now Includes:

1. **Traditional Requirements** (meets original spec)
2. **Extension Questions**:
   - What breaks this solution?
   - How would you test it?
   - What's the performance characteristic?
3. **Design Rationale**: Document *why* you chose this approach
4. **Alternative Approaches**: What else did you consider?

### Grading Rubric Per Activity:
- **60%**: Correctness (traditional flowchart/pseudocode)
- **20%**: Design thinking (extensions)
- **20%**: Communication (clarity, documentation)

---

## Teaching Methodology Changes

### 1. **Show, Don't Just Tell**
Every concept paired with:
- How it looks in pseudocode (required)
- How it maps to real code (Python/C example)
- Where it appears in production systems (e.g., "this is how Netflix handles X")

### 2. **Case Studies Over Lectures**
- Week 1: Show GitHub issue → problem decomposition → PR
- Week 4: Real bug postmortems → trace to decision tree failures
- Week 10: Analyze Uber's surge pricing state machine

### 3. **Reverse Engineering**
- Give students working code → ask them to create flowcharts/pseudocode
- Builds translation skills both directions

### 4. **Collaborative Design**
- Pair activities: One designs, one reviews
- Introduce code review culture early

---

## Tools Introduction (No Hands-On Required, Conceptual Only)

### Week 1: Version Control Concepts
- Why: Collaboration, history, rollback
- Not Git commands, but the mental model

### Week 3: Testing Frameworks
- Unit tests, integration tests (concepts)
- How assertions work

### Week 5: Profilers & Debuggers
- How to measure performance
- How to trace execution

### Week 8: Database Tools
- ORMs, query builders (what they do)
- Why abstraction layers exist

### Week 10: Monitoring & Observability
- Logs, metrics, traces (concepts)
- How to debug production

**Philosophy**: Students should know these exist and *why* they exist before being forced to use them

---

## Sample Enhanced Activity

### Activity 2 (Week 3): Email & Rainfall - Professional Edition

#### Part A: Traditional Requirements (60% of grade)
*[Original requirements unchanged]*

#### Part B: Design Extensions (20% of grade)

**Email System**:
1. What happens if the email server is down when SendEmail is called?
2. Should SendEmail be synchronous or asynchronous? Why?
3. Design a retry mechanism (pseudocode)
4. How would you test SendEmail without sending real emails?

**Rainfall System**:
1. What if a user enters -50mm for rainfall? Handle in pseudocode.
2. How would you modify your solution to handle 100 years instead of 3?
3. Sketch a database schema that could store this data
4. What's the time complexity of your calculations?

#### Part C: Communication (20% of grade)

**Required Documentation**:
- Function contracts (inputs, outputs, side effects)
- Assumptions made
- Edge cases identified
- Design decisions & tradeoffs

**README-style writeup**:
- What does this solve?
- How to use it?
- What are its limitations?

---

## Student Success Metrics

### Beyond Grades:

**Portfolio Building**:
- Best activity solutions → public GitHub repo (optional, encouraged)
- Build a "systems design journal" throughout term

**Skills Developed**:
1. **Computational thinking** (original goal)
2. **System design thinking** (new)
3. **Technical communication** (new)
4. **Design critique** (new)
5. **Professional awareness** (new)

**Career Readiness**:
- Understand what software engineers actually do
- Prepared for technical interviews (system design rounds)
- Can discuss architectural tradeoffs
- Know what DevOps means (culturally, not just tools)

---

## Addressing the "Artificial Constraints" Problem

### The Current Approach:
Professor: "Don't use arrays for this problem"  
Student: "Why not?"  
Professor: "Because I said so" / "You'll learn them later"  
**Result**: Confusion, resentment, missed learning

### The Professional Approach:

**Week 3 Example**:  
*Problem: Sum 10 numbers entered by user*

**The Constrained Way** (meets requirement):
```
FUNCTION SumTenNumbers()
    VARIABLE: num1, num2, num3, num4, num5, num6, num7, num8, num9, num10 (REAL)
    VARIABLE: sum (REAL)
    
    INPUT num1, num2, ... num10
    sum ← num1 + num2 + ... + num10
    RETURN sum
END FUNCTION
```

**Then immediately show**:
```
FUNCTION SumTenNumbers_WithArray()
    VARIABLE: numbers (ARRAY of REAL, size 10)
    VARIABLE: sum (REAL)
    VARIABLE: i (INTEGER)
    
    FOR i ← 0 TO 9 DO
        INPUT numbers[i]
    END FOR
    
    sum ← 0
    FOR i ← 0 TO 9 DO
        sum ← sum + numbers[i]
    END FOR
    
    RETURN sum
END FUNCTION
```

**Discussion**:
- "For this assignment, use the first approach. Here's why we're doing it this way..."
- "In production, you'd use the second. Here's why..."
- "This teaches you to think about data representation before reaching for advanced features"

**Key**: Make the constraint pedagogical, not arbitrary

---

## Integration with DevOps Culture

### Concepts Introduced (No Tooling Required):

**Week 1**: 
- **Version control mindset**: How teams collaborate on code
- **Documentation as code**: README files, inline docs

**Week 4**:
- **Configuration management**: Why hard-coding is bad
- **Environment variables concept**

**Week 6**:
- **Testing pyramid**: Unit → Integration → E2E
- **Test-driven thinking**: Write test cases before implementation

**Week 8**:
- **Database migrations**: How schema changes are managed
- **Backward compatibility**: Why it matters

**Week 10**:
- **Monitoring & alerting**: How to know when things break
- **Incident response**: Postmortems, blameless culture

**Week 11**:
- **CI/CD concepts**: Automated testing, deployment
- **Infrastructure as code**: Servers as cattle not pets

**Throughout**:
- **Code review culture**: Peer feedback on pseudocode
- **Documentation culture**: Every solution needs explanation
- **Systems thinking**: How components interact

---

## Assessment Philosophy

### Original Course:
- Focus: Syntax correctness
- Method: Can you follow notation rules?
- Outcome: Students who can draw flowcharts

### Enhanced Course:
- Focus: Problem-solving + communication
- Method: Can you decompose, design, and explain?
- Outcome: Students who think like engineers

### Grading Mantras:

1. **"Right answer, wrong reasoning" = partial credit**
2. **"Wrong answer, sound reasoning" = substantial credit**
3. **"Right answer, can't explain" = minimal credit**
4. **"Novel approach, well-defended" = full credit + bonus**

---

## Sample Exam Questions (Enhanced)

### Traditional Section (Week 7 Midterm):

**Question 1**: [Standard flowchart/pseudocode problem]

**Question 2 (New)**:  
*You're designing a food delivery system. Sketch the high-level architecture:*
- What are the main components?
- How do they communicate?
- Where could things go wrong?
- How would you handle a restaurant being closed?

*(Graded on reasoning, not perfect solution)*

---

### Final Exam Additions:

**Design Critique Section**:

*Given pseudocode with issues:*
```
FUNCTION ProcessOrder(orderId)
    // Gets customer info
    customer ← DATABASE.query("SELECT * FROM customers")
    
    // Apply discount
    IF customer.email = "admin@test.com" THEN
        discount ← 100
    ELSE
        discount ← 0
    END IF
    
    // Calculate total
    total ← DATABASE.query("SELECT SUM(price) FROM items WHERE orderId=" + orderId)
    finalTotal ← total - discount
    
    // Send email
    SendEmail(customer.email, "Your order total: " + finalTotal)
    
    RETURN "Success"
END FUNCTION
```

**Identify and fix**:
1. Performance issues
2. Security issues
3. Error handling gaps
4. Design flaws
5. Propose refactoring

---

## Resource Recommendations

### Required Reading (Beyond Course Notes):

**Week 1**: 
- "How to Solve It" - Polya (problem decomposition)
- Selected GitHub issue threads (real-world decomposition)

**Week 5**:
- Big O notation guide (conceptual, not mathematical)

**Week 8**:
- Database normalization primer
- Domain-driven design intro

**Week 10**:
- State machine design patterns
- Event-driven architecture overview

**Week 11**:
- Microservices patterns (intro)
- API design best practices

### Optional (Career Building):

- "Designing Data-Intensive Applications" - Kleppmann (skim relevant chapters)
- "The Pragmatic Programmer" - Hunt & Thomas
- System design interview prep resources
- Real engineering blogs (Netflix, Uber, Stripe)

---

## Why This Works Better

### For Students:
1. **Context**: Understand *why* we learn this
2. **Motivation**: See where it's used in real systems
3. **Preparation**: Ready for internships/next courses
4. **Skills**: Actual engineering thinking, not just notation

### For Instructors:
1. **Engagement**: Students care more when they see relevance
2. **Flexibility**: Can show multiple approaches
3. **Assessment**: Can evaluate thinking, not just syntax
4. **Impact**: Students become better problem solvers

### For Industry:
1. **Graduates who think about systems**, not just code
2. **Understand tradeoffs and constraints**
3. **Can communicate technical decisions**
4. **Aware of modern practices**

---

## Implementation Notes

### Minimal Changes to Existing Infrastructure:

**Keep**:
- All activity deadlines
- In-class worksheets
- Grading percentages (mostly)
- Flowchart/pseudocode requirements

**Add**:
- Extension questions to activities (20% of grade)
- Design rationale requirements
- Case study discussions (10-15 min/class)
- "Real-world connection" slides

**Effort Required**:
- Instructors: +2-3 hours prep/week (creating extensions, sourcing case studies)
- Students: +1-2 hours/activity (design thinking, documentation)
- **ROI**: Dramatically better learning outcomes

---

## Migration Path

### Phase 1 (This Term):
- Keep all original requirements
- Add optional "extension challenges" for bonus marks
- Introduce concepts in lectures (no assessment)

### Phase 2 (Next Term):
- Make extensions worth 20% of activity grades
- Add system design component to midterm (10%)
- Update final exam format

### Phase 3 (Future):
- Full integration with follow-on courses
- Coordinate with IPC144/OOP244 instructors
- Build shared case study library

---

## Appendix: Terminology Bridge

**Student asks: "What's the real name for this?"**

| Course Term | Professional Term | Used In |
|------------|------------------|---------|
| Closed-box function | Abstract interface, Black box | API design, testing |
| Data structure | Data model, Schema | Databases, OOP |
| Collection | Container, Data structure | STL, Java Collections |
| Selection | Conditional, Branch | All code |
| Iteration | Loop, Recursion | All code |
| Pattern recognition | Code reuse, DRY | Refactoring |
| Abstraction | Generalization, Polymorphism | OOP, FP |
| Decomposition | Modularization | Architecture |
| Algorithm | Implementation, Logic | Everything |

---

## FAQ for Instructors

**Q: Won't this confuse students with "too much too soon"?**  
A: We're not teaching the tools, we're showing they exist and *why*. Students can handle context better than we think.

**Q: How do I grade "system design" subjectively?**  
A: Rubric focuses on:
- Did they identify key components?
- Did they consider edge cases?
- Can they explain their choices?
- Is the reasoning sound?

Not: "Did they get the perfect answer?"

**Q: What if students just want to pass the tests?**  
A: That's fine. The traditional requirements haven't changed. Extensions are for those who want deeper understanding.

**Q: How do I fit this into 3-hour class blocks?**  
A: 
- 90 min: Traditional content (unchanged)
- 30 min: Case study / real-world connection
- 60 min: Activity work (now includes extensions)

**Q: Won't this disadvantage students with no prior experience?**  
A: No. The core requirements are identical. Extensions reward curiosity, not experience. A thoughtful beginner beats an incurious "expert."

---

## Conclusion

This redesign preserves every original learning objective while adding professional context that makes the material meaningful. Students still master computational thinking, flowcharts, and pseudocode - but now they understand *why* these skills matter and *where* they apply in real systems.

Most importantly: Students leave ready to think like engineers, not just draw flowcharts.