# Markkula Ethics Framework (Claude skill)

A Claude skill that works through an ethical dilemma using the ethical decision-making framework from the Markkula Center for Applied Ethics at Santa Clara University. You describe a situation. Claude asks how you want the answer, tests the decision, looks at it through five ethical lenses at once, lays out four options, and ends with one clear recommendation.

## Important warning: this is a brainstorming tool, not an ethics authority and only applies the framework from the Markkula Center

**AI cannot be ethical, and it cannot make ethical decisions for you.** Claude is a language model. It has no conscience, no moral responsibility, and no stake in what happens to the people affected. It does not understand harm the way a person does, and nobody can hold it accountable for its advice. It can also be wrong, miss facts or stakeholders, repeat biases from the text it learned from, and sound more certain than it should.

Use this skill only to **brainstorm**: to see more of the problem, to surface issues and stakeholders you missed, to test your reasoning from different angles, and to generate options. Do not use it to settle a real ethical question. Business students can use this skill to understand and learn their ethics courses better. They should not use it for solutions in graded and proctored testing.

- The verdicts ("ethical" or "unethical") and the recommendation are prompts for your own thinking. They are not rulings.
- The skill is told to commit to a position so the reasoning is easy to inspect and argue with. A confident answer does not make it correct.
- For a real decision, talk to the people affected and to people who see it differently, and take your own responsibility for the choice. Where the law, a profession's code, or serious harm is involved, ask a qualified professional (a lawyer, an ethics officer, or your professional body).
- Do not use the output as proof that a decision was ethical, or as cover for a decision you have already made.

## The framework behind it

The Markkula Center for Applied Ethics at Santa Clara University has published *A Framework for Ethical Decision Making*, a framework for spotting ethical issues, getting the facts, weighing options through several ethical lenses, choosing, and reflecting afterwards. The Center says the framework has been reprinted in hundreds of articles, books and course materials. It is a classic of business ethics teaching and is commonly used in business and professional ethics courses.

This skill is built on that framework and the Center's essays on its lenses. Everything it teaches about ethics comes from those sources, so it does not mix in other doctrines or slogans. The Center's materials are at https://www.scu.edu/ethics/ethics-resources/ethical-decision-making/

All credit for the framework and the ideas in it belongs to the Markkula Center for Applied Ethics at Santa Clara University. This skill is an independent project. It is not made, reviewed or endorsed by Santa Clara University or the Markkula Center.

## Why this framework

Most people use one rule of thumb to judge a hard decision: what is legal, what most people do, what feels right. The framework starts from the point that none of these is enough. Ethics is not the same as feelings, religion, the law, cultural norms, or science. So instead of one test, it asks you to look at the same decision through several lenses, because each one shows something the others miss:

| Lens | The question it asks |
|---|---|
| Utilitarian | Which option does the most good and the least harm for everyone affected? |
| Rights | Which option best respects the rights of everyone with a stake? |
| Justice | Which option treats people fairly, giving each what they are due? |
| Common good | Which option best serves the community as a whole, not just some members? |
| Care ethics | Which option takes proper account of the relationships, concerns and feelings of everyone involved? |

The lenses are broad strokes, and they sometimes disagree. The framework is honest about this: it does not give an ethics algorithm and does not decide for you. It makes you see more of the problem before you decide.

Virtue ethics another part of the framework is left out because it asks what kind of person you become and what character you build, and that is a question only a human can honestly answer about themselves, so an AI shouldn’t judge it for you.

## What the skill does

1. **Asks two questions first.** How you want the answer (genuine analysis, or a short exam-ready answer) and which perspective to take (company, manager, or personal).
2. **Pins down the case.** It restates the situation, the ethical issues, the known and unknown facts, the stakeholders and the options. If real companies, people, laws or figures are involved, it looks up verified facts and labels anything it could not verify.
3. **Runs a smell test.** Would you be comfortable seeing the decision on the front page of a newspaper, and explaining it to family and friends? If it finds no conundrum, you can accept that or overrule it.
4. **Runs five independent lens agents in parallel.** They are utilitarian, rights, justice, common good and care ethics. They cannot see each other's reports. Each gives a verdict (ethical or unethical), the strongest counterargument and its answer, and works out four options:
   - **Completely ethical:** fully removes the violation, whatever it costs.
   - **Continue as is:** changes nothing, and shows the consequences.
   - **Double down:** escalates or defends the current course, and shows the consequences.
   - **Middle path:** removes or minimises the violation at the lowest cost, and names who pays.
5. **Compares the options and combines the five middle paths** into one, with its cost, the conditions and deadlines, a fallback, and any violation that remains.
6. **Gives a recommendation.** One action, with the reason, plus how to check how it turned out and a plain statement of the framework's limits.

Claude is told to commit and not hedge. Nuance means naming the condition, the cost or the counterargument. It does not mean "arguably" or "it depends".

## Download

This repository has one file you need: `markkula-ethics-framework.skill`.

1. Open this repository on GitHub.
2. Click `markkula-ethics-framework.skill` in the file list.
3. Click the download icon (**Download raw file**) at the top right of the file view. Do not use **Code > Download ZIP** unless you want the whole repository: you only need the single `.skill` file.
4. Save it anywhere on your computer. Do not unzip it. It has to stay as a `.skill` file.

## Install in Claude

1. Open Claude and go to **Settings**, then the **Skills** (or **Capabilities**) section.
2. Upload `markkula-ethics-framework.skill`.
3. Turn the skill on.

## Use it

Describe your dilemma in a message and ask Claude to use the Markkula ethics framework, or type `/markkula-ethics-framework` followed by the situation. Answer the two pop-up questions and Claude does the rest.

Example: `/markkula-ethics-framework` *A supplier we depend on pays its workers below the legal wage. Cancelling the contract would cost us 8% of margin. Should we keep buying from them?*

## Limits

- AI is not an ethical agent. This skill can only help you brainstorm. See the warning at the top.
- The framework does not decide for you. When the lenses disagree, the final weighing is your judgment.
- The lenses are broad-stroke descriptions, and people may not agree on their content, such as which rights exist or what the common good is.
- It is not a full account of ethical thought across history and cultures.
- It works best on a specific case with named actors and a decision to make. For a novel or difficult dilemma, talk it through with people who see it differently.
- When real companies, people, laws or figures are involved, Claude searches the web for facts, so details from your case may appear in search queries.

## License

MIT. See `LICENSE`.
