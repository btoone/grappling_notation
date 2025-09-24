# Grappling Notation

A lightweight symbolic notation for recording grappling events.

## Grappling Notation Specification

[Attacker ↳ Defender] :: Submission @ Position

### Components

- Attacker / Defender: Names, initials, or IDs
- Submission attempt marker: An indicator of a submission attempt (left → right) (`↳`)
- Separator: A separator between actors and metadata (`::`)
- Action: Name of submission or action
- Position: Position context (optional if implicit) (`@`)
- Outcome markers: The result of the action or chain (option) (`!!`)

### Symbols

| Symbol | Meaning |
| ------ | ------- |
|  `↳`   | Submission applied               |
|  `::`  | Actor/Action separator           |
|  `@`   | Position indicator               |
|  `~`   | Transition between positions     |
|  `!!`  | Finished (tap, break, choke out) |
|  `??`  | Failed attempt                   |
|  `>>`  | Sequence/chain of submissions    |
|  `//`  | Comment/annotation               |


### Extended Syntax

#### 1. Transitions

```text
[Gordon ↳ Giancarlo] :: Americana @ Mount ~ SideControl
```

#### 2. Outcomes

```text
[Gordon ↳ Giancarlo] :: Triangle @ Guard !!
[Gordon ↳ Giancarlo] :: Armbar @ Guard ??
```

#### 3. Chains

```text
[Gordon ↳ Giancarlo] :: Kimura >> Armbar @ HalfGuard
```

#### 4. Positional-only

```text
[Gordon] :: GuardPull @ ClosedGuard
```

#### 5. Comments

```text
[Gordon ↳ Giancarlo] :: Guillotine @ Standing // defended by roll
```

## Rule: Outcome Omission

- If no outcome marker (`!!`, `??`) is present, the action or chain is considered unspecified/neutral.
- This records the flow of attempts without stating the result.

### Examples

```text
[Gordon ↳ Giancarlo] :: Kimura >> Armbar @ HalfGuard
[Gordon ↳ Giancarlo] :: Kimura @ SideControl
```

## Abbreviations

- Positions: Mt = Mount, SC = Side Control, HG = Half Guard, G = Guard, 50 = 50/50
- Submissions: Kim = Kimura, Arm = Armbar, Tri = Triangle, RNC = Rear Naked Choke

```text
[GRD ↳ GCL] :: Tri @ G !!
```

## Example Match Log

```text
[Gordon] :: GuardPull @ G
[Gordon ↳ Giancarlo] :: Armbar @ G ??
[Gordon ↳ Giancarlo] :: Triangle @ G !!
```
