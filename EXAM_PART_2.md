<h1 id="part1_intro"><code>Part #2 - Backend</code></h1>
<h2>You have 1 hour for this part of the exam</h2>
<br/>

<h2>Instructions:</h2>
<ul>
    <li>For this part, you only need to work with the existing frontend, but will now also use the DB and Backend instead of your local state</li>
    <li>You are still ALLOWED to use any online resource to help you, including Google, StackOverflow & ChatGPT, you must use them on the shared screen you are using.</li>
    <li>We highly recommend reading all Task requirements before starting each task!</li>
    <li>We care about code quality, style and performance, so it's generally better to finish less tasks, but do them well than to rush through the tasks!</li>
    <li>Please let us know each time a Task is completed, prior to moving on.</li>
</ul>

<br/>

<h2>Exam Part #2 Requirements:</h2>
<h4>Add a new endpoint that receives the task details on submit, and stores it into the DB as a task document into the 'tasks' collection.</h4>
<h4>Display a Toast or other success/failure notification depending on server response</h4>
<h4>Add a 2nd Submit button on the frontend, called 'aSync Submit', which should use a separate server-side endpoint. In this case, the server should simulate a very long process that can take 10 seconds to complete. So the server should respond immediately with a Job ID, and only store the task value to the server after 10 seconds.<h4>
<h4>Frontend should receive the job ID from the server and should update the user once the job has completed with a Toast/Alert message.</h4>
<h4>Card should only show up when the job has completed successfully and should only use the content provided by the server to populate it's state ( not the original form state )</h4>

<h2>Bonus Requirements, if you have time left:</h2>
<h4>Add options to Edit and Delete cards</h4>
<h4>When the async request is sent to the Server, show the Card immediately with a <a href="https://mui.com/material-ui/react-skeleton/">Skeleton</a>.</h4>
<p>If the request fails, remove the card and show the Error Toast \ Alert message and remove the card. If the server returned success, keep the card, change the Skeleton to the actual content received and show a success Toast/Alert message</p>

<br/>

<h3>When done, please commit and push your changes into a new branch called "[YOUR_NAME_TASK_2]" and let us know you're ready for the next task.</h3>
