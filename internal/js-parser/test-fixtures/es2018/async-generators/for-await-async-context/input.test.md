# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `es2018 > async-generators > for-await-async-context`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: true
	directives: Array []
	filename: "es2018/async-generators/for-await-async-context/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "es2018/async-generators/for-await-async-context/input.js"
		end: Object {
			column: 0
			line: 4
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
				message: MARKUP {
					parts: Array [
						RAW_MARKUP {value: "Unexpected token, expected "}
						"("
					]
				}
			}
			location: Object {
				filename: "es2018/async-generators/for-await-async-context/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 11
					line: 2
				}
				start: Object {
					column: 6
					line: 2
				}
			}
		}
	]
	body: Array [
		JSFunctionDeclaration {
			id: JSBindingIdentifier {
				name: "f"
				loc: Object {
					filename: "es2018/async-generators/for-await-async-context/input.js"
					identifierName: "f"
					end: Object {
						column: 10
						line: 1
					}
					start: Object {
						column: 9
						line: 1
					}
				}
			}
			loc: Object {
				filename: "es2018/async-generators/for-await-async-context/input.js"
				end: Object {
					column: 1
					line: 3
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			head: JSFunctionHead {
				async: false
				generator: false
				hasHoistedVars: false
				params: Array []
				rest: undefined
				returnType: undefined
				thisType: undefined
				typeParameters: undefined
				loc: Object {
					filename: "es2018/async-generators/for-await-async-context/input.js"
					end: Object {
						column: 12
						line: 1
					}
					start: Object {
						column: 10
						line: 1
					}
				}
			}
			body: JSBlockStatement {
				directives: Array []
				loc: Object {
					filename: "es2018/async-generators/for-await-async-context/input.js"
					end: Object {
						column: 1
						line: 3
					}
					start: Object {
						column: 13
						line: 1
					}
				}
				body: Array [
					JSForStatement {
						loc: Object {
							filename: "es2018/async-generators/for-await-async-context/input.js"
							end: Object {
								column: 23
								line: 2
							}
							start: Object {
								column: 2
								line: 2
							}
						}
						test: JSReferenceIdentifier {
							name: "x"
							loc: Object {
								filename: "es2018/async-generators/for-await-async-context/input.js"
								identifierName: "x"
								end: Object {
									column: 18
									line: 2
								}
								start: Object {
									column: 17
									line: 2
								}
							}
						}
						update: JSReferenceIdentifier {
							name: "of"
							loc: Object {
								filename: "es2018/async-generators/for-await-async-context/input.js"
								identifierName: "of"
								end: Object {
									column: 21
									line: 2
								}
								start: Object {
									column: 19
									line: 2
								}
							}
						}
						body: JSExpressionStatement {
							loc: Object {
								filename: "es2018/async-generators/for-await-async-context/input.js"
								end: Object {
									column: 23
									line: 2
								}
								start: Object {
									column: 22
									line: 2
								}
							}
							expression: JSReferenceIdentifier {
								name: "y"
								loc: Object {
									filename: "es2018/async-generators/for-await-async-context/input.js"
									identifierName: "y"
									end: Object {
										column: 23
										line: 2
									}
									start: Object {
										column: 22
										line: 2
									}
								}
							}
						}
						init: JSCallExpression {
							loc: Object {
								filename: "es2018/async-generators/for-await-async-context/input.js"
								end: Object {
									column: 16
									line: 2
								}
								start: Object {
									column: 6
									line: 2
								}
							}
							callee: JSReferenceIdentifier {
								name: "await"
								loc: Object {
									filename: "es2018/async-generators/for-await-async-context/input.js"
									identifierName: "await"
									end: Object {
										column: 11
										line: 2
									}
									start: Object {
										column: 6
										line: 2
									}
								}
							}
							arguments: Array [
								JSReferenceIdentifier {
									name: "let"
									loc: Object {
										filename: "es2018/async-generators/for-await-async-context/input.js"
										identifierName: "let"
										end: Object {
											column: 16
											line: 2
										}
										start: Object {
											column: 13
											line: 2
										}
									}
								}
							]
						}
					}
					JSExpressionStatement {
						loc: Object {
							filename: "es2018/async-generators/for-await-async-context/input.js"
							end: Object {
								column: 25
								line: 2
							}
							start: Object {
								column: 23
								line: 2
							}
						}
						expression: JSReferenceIdentifier {
							name: "INVALID_PLACEHOLDER"
							loc: Object {
								filename: "es2018/async-generators/for-await-async-context/input.js"
								end: Object {
									column: 24
									line: 2
								}
								start: Object {
									column: 23
									line: 2
								}
							}
						}
					}
				]
			}
		}
	]
}
```

### `diagnostics`

```

 es2018/async-generators/for-await-async-context/input.js:2:6 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Unexpected token, expected (

    1 │ function f() {
  > 2 │   for await (let x of y);
      │       ^^^^^
    3 │ }

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```
