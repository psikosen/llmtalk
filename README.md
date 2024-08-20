# Expanded LLMTalk DSL Syntax

## 1. General Structure
- Command Structure: `[TOPIC]:[ACTION] : [DETAILS]`
- Details are specified in square brackets: `[KEY=VALUE]`

## 2. Universal Modifiers
These can be applied to most commands:
- `[DETAILS=FORMAT, BEST_PRACTICES]`: Ensures output follows best practices and is properly formatted
- `[COMMENTS=YES/NO]`: Specifies whether to include comments in the output
- `[LENGTH=short/medium/long]`: Specifies the desired length of the content
- `[DEPTH=basic/advanced]`: Indicates the level of detail or complexity
- `[LANGUAGE=language]`: Specifies the output language
- `[FORMAT=format]`: Specifies the output format (e.g., markdown, plain text, LaTeX)

## 3. Coding Commands

### 3.1 Writing Code
```
CODE_WRITE:Function : [LANGUAGE=language] [TASK=task] [DETAILS=FORMAT, BEST_PRACTICES, COMMENTS=YES/NO]
```

### 3.2 Explaining Code
```
CODE_EXPLAIN:Snippet : [LANGUAGE=language] [CODE=code] [DETAILS=BEST_PRACTICES, COMMENTS=YES/NO]
```

### 3.3 Refactoring Code
```
CODE_REFACTOR:Snippet : [LANGUAGE=language] [CODE=code] [DETAILS=FORMAT, BEST_PRACTICES, COMMENTS=YES/NO]
```

### 3.4 Testing Code
```
CODE_TEST:Function : [LANGUAGE=language] [TASK=task] [DETAILS=BEST_PRACTICES]
```

### 3.5 Debugging Code
```
CODE_DEBUG:Snippet : [LANGUAGE=language] [CODE=code] [DETAILS=IDENTIFY_ISSUES, SUGGEST_FIXES, COMMENTS=YES/NO]
```

### 3.6 Documenting Code
```
CODE_DOC:Function : [LANGUAGE=language] [CODE=code] [DETAILS=INCLUDE_EXAMPLES, COMMENTS=YES/NO]
```

### 3.7 Version Control
```
CODE_VCS:Task : [LANGUAGE=language] [ACTION=commit/branch/merge] [DETAILS=DETAILS]
```

### 3.8 Optimizing Code
```
CODE_OPTIMIZE:Snippet : [LANGUAGE=language] [CODE=code] [DETAILS=PERFORMANCE, MEMORY_USAGE]
```

### 3.9 Security Checks
```
CODE_SECURE:Snippet : [LANGUAGE=language] [CODE=code] [DETAILS=VULNERABILITY_SCAN]
```

### 3.10 Style/Linting
```
CODE_LINT:Snippet : [LANGUAGE=language] [CODE=code] [DETAILS=BEST_PRACTICES]
```

### 3.11 Code Snippet Management
```
CODE_SNIPPET:Task : [ACTION=save/retrieve/manage] [CODE=code]
```

### 3.12 Code Comparison
```
CODE_COMPARE:Versions : [CODE1=first snippet] [CODE2=second snippet]
```

### 3.13 Code Merging
```
CODE_MERGE:Versions : [SOURCE=source code] [DESTINATION=destination code] [DETAILS=RESOLVE_CONFLICTS]
```

### 3.14 Code Generation
```
CODE_GENERATE:Type : [LANGUAGE=language] [FRAMEWORK=framework] [DETAILS=STRUCTURE, FUNCTIONALITY]
```

### 3.15 API Integration
```
CODE_API:Integration : [API=api_name] [ENDPOINT=endpoint] [DETAILS=AUTHENTICATION, PARAMETERS]
```

## 4. Writing Commands

### 4.1 General Writing
```
WRITE:Content : [FORMAT=essay/report/email/blog post/story] [TONE=tone] [LENGTH=length] [STRUCTURE=structure]
```

### 4.2 Creative Writing
```
WRITE:Story : [PERSPECTIVE=first/second/third] [STYLE=style] [LENGTH=length]
```

### 4.3 Tone and Audience
```
WRITE:Content : [TONE=casual/formal/professional/creative] [AUDIENCE=general/specific]
```

### 4.4 Specific Elements and Features
```
WRITE:Content : [USE_HEADINGS=YES/NO] [INCLUDE_SOURCES=YES/NO] [INCLUDE_QUOTES=YES/NO]
```

### 4.5 Style and Structure
```
WRITE:Content : [STYLE=descriptive/persuasive/narrative/expository] [STRUCTURE=intro-body-conclusion/chronological/point-by-point]
```

### 4.6 Content Editing
```
EDIT:Content : [TYPE=grammar/style/structure] [LEVEL=light/moderate/heavy]
```

### 4.7 Content Summarization
```
SUMMARIZE:Content : [LENGTH=short/medium/long] [FOCUS=key points/main ideas/conclusions]
```

### 4.8 Content Translation
```
TRANSLATE:Content : [SOURCE_LANG=language] [TARGET_LANG=language] [STYLE=literal/idiomatic]
```

## 5. Mathematical Commands

### 5.1 Explaining Mathematical Concepts
```
MATH_EXPLAIN:Concept : [TOPIC=topic] [DETAILS=Feynman, LaTeX]
```

### 5.2 Displaying Formulas
```
FORMULA:Equation : [CONTENT=formula] [FORMAT=LaTeX]
```

### 5.3 Deriving Formulas
```
DERIVE:Equation : [TOPIC=topic] [DETAILS=Feynman, LaTeX]
```

### 5.4 Solving Equations
```
SOLVE:Equation : [EQUATION=equation] [METHOD=method] [DETAILS=LaTeX]
```

### 5.5 Graphing Functions
```
GRAPH:Function : [FUNCTION=function] [RANGE=range] [DETAILS=LaTeX]
```

### 5.6 Calculating Derivatives and Integrals
```
CALCULATE:Derivative/Integral : [FUNCTION=function] [POINT=point] [DETAILS=LaTeX]
```

### 5.7 Simplifying Expressions
```
SIMPLIFY:Expression : [EXPRESSION=expression] [DETAILS=LaTeX]
```

### 5.8 Explaining Theorems
```
EXPLAIN_THEOREM:Theorem : [TOPIC=theorem] [DETAILS=Feynman, LaTeX]
```

### 5.9 Additional Math Details
- `[EXPLANATION=TEXT]`: Provides a plain text explanation
- `[STEPS=YES]`: Breaks down the process into clear steps
- `[VISUAL=YES]`: Generates accompanying visual aids
- `[INTERACTIVE=YES]`: Provides an interactive component
- `[PROOF=YES]`: Provides a formal mathematical proof
- `[CONTEXT=YES]`: Adds background or contextual information
- `[EXAMPLES=YES]`: Provides real-world applications or examples
- `[SIMPLIFIED=YES]`: Ensures the explanation is in a simplified form
- `[SYMBOLIC=YES]`: Focuses on symbolic manipulation and output
- `[LANGUAGE=language]`: Provides the explanation in a different language

### 5.10 Statistical Analysis
```
STATS:Analysis : [DATA=dataset] [TEST=statistical_test] [DETAILS=ASSUMPTIONS, INTERPRETATION]
```

### 5.11 Probability Calculations
```
PROBABILITY:Calculate : [EVENT=event] [DISTRIBUTION=distribution] [DETAILS=PARAMETERS, METHOD]
```

## 6. Specialized Commands

### 6.1 Medical Summarization
```
MEDICAL_SUMMARY:Patient Information : [DETAILS=SOAP]
```

### 6.2 Scientific Research Summarization
```
SCIENCE_SUMMARY:Study Information : [DETAILS=METHODS, RESULTS, CONCLUSION, FORMAT=LaTeX]
```

### 6.3 Legal Analysis
```
LEGAL_ANALYSIS:Case Information : [DETAILS=KEY_ISSUES, ARGUMENTS, OUTCOMES]
```

### 6.4 Business Reports
```
BUSINESS_REPORT:Financial Information : [DETAILS=SUMMARY, TRENDS, RECOMMENDATIONS, FORMAT=CHARTS]
```

### 6.5 Educational Content Creation
```
EDUCATIONAL_CONTENT:Lesson Information : [SUBJECT=subject] [GRADE_LEVEL=level] [DETAILS=OBJECTIVES, ACTIVITIES, ASSESSMENT]
```

### 6.6 Project Management
```
PROJECT_PLAN:Project Information : [DETAILS=TIMELINE, MILESTONES, RESOURCES]
```

### 6.7 Data Analysis
```
DATA_ANALYSIS:Dataset Information : [DETAILS=SUMMARY, TRENDS, VISUALIZATIONS]
```

### 6.8 Historical Analysis
```
HISTORICAL_ANALYSIS:Event Information : [DETAILS=CAUSES, EFFECTS, SIGNIFICANCE]
```

### 6.9 Personal Finance Summary
```
FINANCE_SUMMARY:Financial Information : [DETAILS=INCOME, EXPENSES, SAVINGS, RECOMMENDATIONS]
```

### 6.10 Creative Story Generation
```
CREATE_STORY:Character : [TYPE=character type] [GOAL=character goal] [THEME=story theme] [TONE=story tone]
```

### 6.11 Market Research
```
MARKET_RESEARCH:Topic : [INDUSTRY=industry] [SCOPE=local/global] [DETAILS=TRENDS, COMPETITORS, OPPORTUNITIES]
```

### 6.12 Environmental Impact Assessment
```
ENVIRONMENT_IMPACT:Project : [TYPE=project type] [LOCATION=location] [DETAILS=ECOSYSTEM, MITIGATION, LONG_TERM_EFFECTS]
```

### 6.13 Psychological Profile
```
PSYCH_PROFILE:Subject : [TRAITS=trait list] [BEHAVIOR=observed behaviors] [DETAILS=ANALYSIS, RECOMMENDATIONS]
```