# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `typescript > cast > destructure-and-assign`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "typescript/cast/destructure-and-assign/input.ts"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "module"
	syntax: Array ["ts"]
	loc: Object {
		filename: "typescript/cast/destructure-and-assign/input.ts"
		end: Object {
			column: 0
			line: 3
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Unexpected type cast in parameter position"}]}
			}
			location: Object {
				filename: "typescript/cast/destructure-and-assign/input.ts"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 12
					line: 1
				}
				start: Object {
					column: 1
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "typescript/cast/destructure-and-assign/input.ts"
				end: Object {
					column: 21
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			expression: JSAssignmentExpression {
				operator: "="
				loc: Object {
					filename: "typescript/cast/destructure-and-assign/input.ts"
					end: Object {
						column: 20
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
				right: JSArrayExpression {
					loc: Object {
						filename: "typescript/cast/destructure-and-assign/input.ts"
						end: Object {
							column: 20
							line: 1
						}
						start: Object {
							column: 16
							line: 1
						}
					}
					elements: Array [
						JSNumericLiteral {
							value: 42
							format: undefined
							loc: Object {
								filename: "typescript/cast/destructure-and-assign/input.ts"
								end: Object {
									column: 19
									line: 1
								}
								start: Object {
									column: 17
									line: 1
								}
							}
						}
					]
				}
				left: JSAssignmentArrayPattern {
					rest: undefined
					loc: Object {
						filename: "typescript/cast/destructure-and-assign/input.ts"
						end: Object {
							column: 13
							line: 1
						}
						start: Object {
							column: 0
							line: 1
						}
					}
					elements: Array [
						TSAssignmentAsExpression {
							loc: Object {
								filename: "typescript/cast/destructure-and-assign/input.ts"
								end: Object {
									column: 12
									line: 1
								}
								start: Object {
									column: 1
									line: 1
								}
							}
							typeAnnotation: TSNumberKeywordTypeAnnotation {
								loc: Object {
									filename: "typescript/cast/destructure-and-assign/input.ts"
									end: Object {
										column: 12
										line: 1
									}
									start: Object {
										column: 6
										line: 1
									}
								}
							}
							expression: JSAssignmentIdentifier {
								name: "a"
								loc: Object {
									filename: "typescript/cast/destructure-and-assign/input.ts"
									identifierName: "a"
									end: Object {
										column: 2
										line: 1
									}
									start: Object {
										column: 1
										line: 1
									}
								}
							}
						}
					]
				}
			}
		}
		JSExpressionStatement {
			loc: Object {
				filename: "typescript/cast/destructure-and-assign/input.ts"
				end: Object {
					column: 19
					line: 2
				}
				start: Object {
					column: 0
					line: 2
				}
			}
			expression: JSAssignmentExpression {
				operator: "="
				loc: Object {
					filename: "typescript/cast/destructure-and-assign/input.ts"
					end: Object {
						column: 18
						line: 2
					}
					start: Object {
						column: 0
						line: 2
					}
				}
				right: JSArrayExpression {
					loc: Object {
						filename: "typescript/cast/destructure-and-assign/input.ts"
						end: Object {
							column: 18
							line: 2
						}
						start: Object {
							column: 14
							line: 2
						}
					}
					elements: Array [
						JSNumericLiteral {
							value: 42
							format: undefined
							loc: Object {
								filename: "typescript/cast/destructure-and-assign/input.ts"
								end: Object {
									column: 17
									line: 2
								}
								start: Object {
									column: 15
									line: 2
								}
							}
						}
					]
				}
				left: JSAssignmentArrayPattern {
					rest: undefined
					loc: Object {
						filename: "typescript/cast/destructure-and-assign/input.ts"
						end: Object {
							column: 11
							line: 2
						}
						start: Object {
							column: 0
							line: 2
						}
					}
					elements: Array [
						TSAssignmentTypeAssertion {
							loc: Object {
								filename: "typescript/cast/destructure-and-assign/input.ts"
								end: Object {
									column: 10
									line: 2
								}
								start: Object {
									column: 1
									line: 2
								}
							}
							typeAnnotation: TSNumberKeywordTypeAnnotation {
								loc: Object {
									filename: "typescript/cast/destructure-and-assign/input.ts"
									end: Object {
										column: 8
										line: 2
									}
									start: Object {
										column: 2
										line: 2
									}
								}
							}
							expression: JSAssignmentIdentifier {
								name: "a"
								loc: Object {
									filename: "typescript/cast/destructure-and-assign/input.ts"
									identifierName: "a"
									end: Object {
										column: 10
										line: 2
									}
									start: Object {
										column: 9
										line: 2
									}
								}
							}
						}
					]
				}
			}
		}
	]
}
```

### `diagnostics`

```

 typescript/cast/destructure-and-assign/input.ts:1:1 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Unexpected type cast in parameter position

  > 1 │ [a as number] = [42];
      │  ^^^^^^^^^^^
    2 │ [<number>a] = [42];

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```
