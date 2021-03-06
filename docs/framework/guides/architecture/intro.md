---
category: framework-architecture
order: 10
---

# Introduction

This guide introduces the main pilars of CKEditor 5 architecture. It is assumed that you have read the {@link framework/guides/overview Framework's overview} and saw some code in the {@link framework/guides/quick-start Quick start} guide. This should help you going through the next steps.

## Main pilars

CKEditor 5 framework comes with its 3 main pilars:

* **{@link framework/guides/architecture/core-editor-architecture Core editor architecture}**

	The core editor architecture is implemented by the {@link api/core `@ckeditor/ckeditor5-core`} package. It consists of a couple of core classes and interfaces that glue everything together.

	The main purpose of the editor architecture is to lay the groundwork for implementing editor features. Therefore, it introduces concepts such as {@link framework/guides/architecture/core-editor-architecture#plugins plugins} and {@link framework/guides/architecture/core-editor-architecture#commands commands} which simplify and standardize the way to implementing features.

* **{@link framework/guides/architecture/editing-engine Editing engine}**

	The editing engine is implemented by the {@link api/engine `@ckeditor/ckeditor5-engine`} package. It is the biggest and by far most complex pilar of the framework, implementing the custom data model, the view layer, conversion mechanisms, rendering engine responsible for [taming `contentEditable`](https://medium.com/content-uneditable/contenteditable-the-good-the-bad-and-the-ugly-261a38555e9c) and a lot more.

* **{@link framework/guides/architecture/ui-library UI library}**

	The standard UI library is implemented by the {@link api/ui `@ckeditor/ckeditor5-ui`} package. It contains a simple MVC implementation whose main goal is to best fit CKEditor 5 needs. Furthermore, it introduces basic UI components to be used by editor features.
