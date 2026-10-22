<h2>Module 1: Intro to AI</h2>

<h2>Module 2: Pair-coding with an LLM</h2>

<h3>Lesson 1: Assigning the LLM a role</h3>

<h4>Prompt with role assignment</h4>
<b>Examples</b>
<li>As a beginner Python tutor, explain how to crete a list in Oython and add elements to it.</li> 
<li>You are a friendly coding mentor. Explain how to create a list in Python and add elements to it.</li>
<li>As a friendly code guide, explain how loops work in Python</li> 

<h3>Lesson 2: Leveling up with multiple roles</h3>
<b>Examples</b>
<li>As both a software architect and a security expert, evaluate this Python script for a web application and suggest architectural improvements and security enhancements.</li><br />

```python
def storeuserdata(user_data):
  database = open('user_database.txt', 'a')
  database.write(str(user_data))
  database.close()

storeuserdata({'username': 'admin', 'password': '1234'})
```

<h3>Lesson 3: Expert roles for specialized knowledge</h3>
<b>Examples</b>
Expert role: open source contributor
<li>As a contributor to open-source Python projects, critique this Python library for data visualization and suggest enhancements to make it comparable to major libraries like Matplotlib or Seaborn.</li><br />

```python
import matplotlib.pyplot as plt
class DataVisualizer:
  def init(self, data)
    self.data = data
  def plot(self, kind='line'):
    if kind == 'line':
      plt.plot(self.data)
    elif kind == 'bar':
      plt.bar(range(len(self.data)), self.data)
    plt.show()
#Example usage
visualizer = DataVisualizer([10, 20, 30, 40, 50])
visualizer.plot('bar')
```

Expert role: NLP expert
<li>As an NLP expert, suggest improvement to this text summarization feature to enhance its functionality and accuracy.</li><br />

```python
import nltk
class TextAnalyzer:
  def(init(self, text):
    self.text = text
  def summarize(self):
    sentences = nltk.senttokenize(self.text)
return ' '.join(sentences[:2])
```

Expert role: Software tester
<li>As a software tester, analyze this function for potential edge cases and suggest robust handling strategies.</li><br />

```python
def calculatediscount(price, discount):
  if discount > 100:
    raise ValueError('Discount cannot exceed 100%')
  return price * (100 - discount) / 100
# Test cases
print(calculatediscount(100, 105)) # Should raise an exception
```

<h3>Lesson 4: Pair coding with an LLM (Best practices)</h3>
<li><b>Be specific:</b> Provide detail and context about your problem</li>
<li><b>Assign a role:</b> Assign a role to tailor the output you receive</li>
<li><b>Request an expert opinion:</b> Assign an expert role and ask the LLM to evaluate work you've already done to further refine it</li>
<li><b>Give feedback:</b> Iteratively prompt the LLM and provide feedback on the output you receive to get closer to your expected results</li>

<br />
<h3>Lesson 5: LLM-Powered Coding Tools</h3>

<table>
  <!-- Header Row (Defines the 3 column titles) -->
  <thead>
    <tr>
      <th>Stand-alone Chat</th>
      <th>IDE-Integrated</th>
      <th>Agentic</th>
    </tr>
  </thead>
  
  <!-- Body Rows (The actual data) -->
  <tbody>
    <tr>
      <td>LLM runs entirely outside your IDE</td>
      <td>LLM runs inside your IDE</td>
      <td>LLM autonomously interacts with your codebase</td>
    </tr>
    <tr>
      <td>Only know information you share directly with the LLM</td>
      <td>Able to read open files and errors</td>
      <td>One prompt can lead to many actions</td>
    </tr>
      <tr>
      <td>Some LLMs may still search the web</td>
      <td>Easily accept or reject edits</td>
      <td>Can be operated from the command line or UI in your IDE</td>
      </tr>
     <tr>
      <td>You decide how to use responses, and must manually copy-paste in generated code</td>
      <td>Automates gathering relevant context and applying results</td>
      <td>Looks like another developer navigating your codebase</td>
      </tr>
     <tr>
      <td>You completely control the LLM and your codebase</td>
      <td>You move more quickly, but still drive the overall process</td>
      <td>Can read, edit, and delete files, run code to test how it works, or answer questions</td>
      </tr>
      <tr>
      <td></td>
      <td></td>
      <td>Highest level of automation</td>
      </tr>
  </tbody>
</table>

  <!-- 

<ul>
<li>Stand-alone Chat
<ul>
  <li>LLM runs entirely outside your IDE</li>
  <li>Only know information you share directly with the LLM</li>
  <li>Some LLMs may still search the web</li>
  <li>You decide how to use responses, and must manually copy-paste in generated code</li>
  <li>You completely control the LLM and your codebase</li>
</ul>
  
</ul>
<li>IDE-Integrated</li>
<ul>
  <li>LLM runs inside your IDE</li>
  <li>Able to read open files and errors</li>
  <li> Easily accept or reject edits</li>
  <li>Automates gathering relevant context and applying results</li>
  <li>You move more quickly, but still drive the overall process</li>
</ul>

<ul>
<li>Agentic</li>
<ul>
<li>LLM autonomously interacts with your codebase</li>
<li>One prompt can lead to many actions</li>
<li>Can be operated from the command line or UI in your IDE</li>
<li>Looks like another developer navigating your codebase</li>
<li>Can read, edit, and delete files, run code to test how it works, or answer questions</li>
  
</ul>
-->

</ul>
<h3>Lesson 6: LLM-Powered Coding Tools: Strengths and Weaknesses</h3>
https://learn.deeplearning.ai/specializations/generative-ai-for-software-development/lesson/mmxyiw/llm-powered-coding-tools%3A-strengths-and-weaknesses

<h3>Lesson 7: The Context Window</h3>
<li>Longest token sequence a model can process</li>
<li>Range from ~16,000 tokens to 1,000,000+</li>
<li>That's 25 to 1,500 pages</li>
<li>May seem large, but it can be used up quickly</li>

<br />
<td style="background-color: red">LLM Have no memory</td>
<li>LLMs don't remember previous prompts or responses</li>
<li>Ongoing conversations are saved in a "chat history"</li>
<li>When you send a prompt, the entire chat history is also included so the model knows what was said</li>
<li>As conversations continue, more of the context window is used up</li>

<br />
<br />
https://learn.deeplearning.ai/specializations/generative-ai-for-software-development
