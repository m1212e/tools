# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `esprima > invalid-syntax > migrated_0075`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "esprima/invalid-syntax/migrated_0075/input.js"
	hasHoistedVars: false
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "esprima/invalid-syntax/migrated_0075/input.js"
		end: Object {
			column: 0
			line: 2
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
				message: MARKUP {parts: Array [RAW_MARKUP {value: "setter should have exactly one param"}]}
			}
			location: Object {
				filename: "esprima/invalid-syntax/migrated_0075/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 14
					line: 1
				}
				start: Object {
					column: 3
					line: 1
				}
			}
		}
	]
	body: Array [
		JSExpressionStatement {
			loc: Object {
				filename: "esprima/invalid-syntax/migrated_0075/input.js"
				end: Object {
					column: 17
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			expression: JSObjectExpression {
				loc: Object {
					filename: "esprima/invalid-syntax/migrated_0075/input.js"
					end: Object {
						column: 16
						line: 1
					}
					start: Object {
						column: 1
						line: 1
					}
				}
				properties: Array [
					JSObjectMethod {
						kind: "set"
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "s"
								loc: Object {
									filename: "esprima/invalid-syntax/migrated_0075/input.js"
									identifierName: "s"
									end: Object {
										column: 8
										line: 1
									}
									start: Object {
										column: 7
										line: 1
									}
								}
							}
							loc: Object {
								filename: "esprima/invalid-syntax/migrated_0075/input.js"
								end: Object {
									column: 8
									line: 1
								}
								start: Object {
									column: 7
									line: 1
								}
							}
						}
						loc: Object {
							filename: "esprima/invalid-syntax/migrated_0075/input.js"
							end: Object {
								column: 14
								line: 1
							}
							start: Object {
								column: 3
								line: 1
							}
						}
						body: JSBlockStatement {
							body: Array []
							directives: Array []
							loc: Object {
								filename: "esprima/invalid-syntax/migrated_0075/input.js"
								end: Object {
									column: 14
									line: 1
								}
								start: Object {
									column: 11
									line: 1
								}
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
								filename: "esprima/invalid-syntax/migrated_0075/input.js"
								end: Object {
									column: 10
									line: 1
								}
								start: Object {
									column: 8
									line: 1
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

 esprima/invalid-syntax/migrated_0075/input.js:1:3 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ setter should have exactly one param

    ({ set s() { } })
       ^^^^^^^^^^^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```