<template>
  <panel>
    <div slot="title">{{$t('m.Frequently_Asked_Questions')}}</div>
    <div class="content markdown-body">
      <ul>
        <li>Where is the input and the output?
          <p>Your program shall read input from <code>stdin</code>('Standard Input') and write output to <code>stdout</code>('Standard Output').
            For example, in C you can use <code>scanf</code> to read from stdin, and use <code>printf</code> to write to stdout.
            User programs are not allowed to read or write files, or you will get a <code>Runtime Error</code>.
          </p>
        </li>
        <li>What's the meaning of the submission execution time?
        <p>The onlinejudge might test your code multiple times with different input files.
          If your code gives the correct answer within the time limit for each input file, the execution time displayed is the max of the time spent for each test case.
          Otherwise, the execution time will not make sense.
        </p>
        </li>
        <li>About presentation error?
          <p>There is no presentation error in this oj. The judger will trim the blacks and wraps in your ouput's <b>last</b> line.
            If it is still different than the correct output, the result will be <code>Wrong Answer</code>.</p>
        </li>
        <li>How to report bugs about this oj?
          <p>The onlinejudge is open source, you can open an issue in <a href="https://github.com/jachinte/OnlineJudge">Github</a>.
            The details(like env, version..) about a bug are required. These details will help us to solve the bug.
          </p>
        </li>
      </ul>
    </div>
  </panel>
</template>

<script>
</script>

<style lang="less" scoped>
  .content {
    font-size: 16px;
    margin: 0 50px 40px 50px;
    > ul {
      list-style: disc;
      li {
        font-size: 16px;
        margin-top: 20px;
        &:first-child {
          margin-top: 0;
        }
        p {
          font-size: 14px;
          margin-top: 5px;
        }
      }
    }
  }
</style>
