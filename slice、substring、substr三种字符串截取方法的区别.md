1. substring() 方法用于提取字符串中介于两个指定下标之间的字符。  
    ``` 
    stringObject.substring(start,stop)
    ```  
    <table>
      <tr>
        <th>参数</th>
        <th>描述</th>
      </tr>
      <tr>
        <td>start</td>
        <td>必需。一个非负的整数，规定要提取的子串的第一个字符在 stringObject 中的位置。</td>
      </tr>
      <tr>
        <td>stop</td>
        <td>可选。一个非负的整数，比要提取的子串的最后一个字符在 stringObject 中的位置多 1。</td>
      </tr>
    </table>  
    与 slice() 和 substr() 方法不同的是，substring() 不接受负的参数。
2. substr() 方法可在字符串中抽取从 start 下标开始的指定数目的字符。  
    ```
    stringObject.substr(start,length)
    ```
      <table>
          <tr>
            <th>参数</th>
            <th>描述</th>
          </tr>
          <tr>
            <td>start</td>
            <td>必需。要抽取的子串的起始下标。必须是数值。如果是负数，那么该参数声明从字符串的尾部开始算起的位置。也就是说，-1 指字符串中最后一个字符，-2 指倒数第二个字符，以此类推。</td>
          </tr>
          <tr>
            <td>stop</td>
            <td>可选。子串中的字符数。必须是数值。如果省略了该参数，那么返回从 stringObject 的开始位置到结尾的字串。</td>
          </tr>
        </table> 
  3. slice() 方法可提取字符串的某个部分，并以新的字符串返回被提取的部分。  
        ```
     stringObject.slice(start,end)   
        ```   
        <table>
                <tr>
                  <th>参数</th>
                  <th>描述</th>
                </tr>
                <tr>
                  <td>start</td>
                  <td>要抽取的片断的起始下标。如果是负数，则该参数规定的是从字符串的尾部开始算起的位置。也就是说，-1 指字符串的最后一个字符，-2 指倒数第二个字符，以此类推。</td>
                </tr>
                <tr>
                  <td>end</td>
                  <td>紧接着要抽取的片段的结尾的下标。若未指定此参数，则要提取的子串包括 start 到原字符串结尾的字符串。如果该参数是负数，那么它规定的是从字符串的尾部开始算起的位置。</td>
                </tr>
              </table>   
## 总结    
 String 对象的方法 slice()、substring() 和 substr() （不建议使用）都可返回字符串的指定部分。slice() 比 substring() 要灵活一些，因为它允许使用负数作为参数。slice() 与 substr() 有所不同，因为它用两个字符的位置来指定子串，而 substr() 则用字符位置和长度来指定子串。        