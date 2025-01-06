# Sequence Diagrams

Sequence diagrams show how processes operate with one another and in what order.

## Basic Syntax

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->>Bob: Hello Bob, how are you?
    Bob-->>Alice: Great!
    Alice-)Bob: See you later!
```

## Arrow Types

```mermaid
sequenceDiagram
    A->>B: Solid line with arrow
    B-->>A: Dashed line with arrow
    A--->B: Solid line with open arrow
    B---->A: Dashed line with open arrow
    A-)B: Solid line with cross
    B--)A: Dashed line with cross
```

## Activations

```mermaid
sequenceDiagram
    Alice->>+John: Hello John, how are you?
    John-->>-Alice: Great!
    Alice->>+John: See you later!
    John-->>-Alice: Bye!
```

## Notes

```mermaid
sequenceDiagram
    participant John
    participant Alice
    Note right of John: Text right of John
    Note left of Alice: Text left of Alice
    Note over John,Alice: Text over both
```

## Loops

```mermaid
sequenceDiagram
    Alice->John: Hello
    loop Every minute
        John-->Alice: Great!
    end
```

## Alt and Opt

```mermaid
sequenceDiagram
    Alice->>Bob: Hello Bob
    alt is sick
        Bob->>Alice: Not so good :(
    else is well
        Bob->>Alice: Feeling fresh like a daisy
    end
    opt Extra response
        Bob->>Alice: Thanks for asking
    end
```

