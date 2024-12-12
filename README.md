# Tailwind CSS @apply Directive Bug

This repository demonstrates a bug encountered when using Tailwind's `@apply` directive inside a custom directive.  The `@apply` directive sometimes fails to apply the specified styles correctly, leading to inconsistent styling across different screen sizes.

## Problem Description

The primary problem is the unpredictable behavior of `@apply` when embedded within a custom class or a directive.  This makes debugging and maintaining styles challenging.  This can occur when using the `@apply` directive with media queries or other modifiers. 

## Solution

The suggested solution involves refactoring to use regular Tailwind classes directly, eliminating the reliance on `@apply` within the custom directive.   This ensures that Tailwind can process the styles consistently and reliably.