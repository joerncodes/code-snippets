Technology:[[Typescript]]

In TypeScript, you can define the possible values of a string in an interface by using `keyof typeof` with an object:

```typescript
export const TASK_STATES = {
	open: 1,
	inProgress: 2,
	done: -1
}

interface Task {
	status: keyof typeof TASK_STATES;
}
```