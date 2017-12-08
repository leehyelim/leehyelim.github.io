
scope="row" 와 scope="col" 을 붙이는 이유는 쉽게 말해 스크린 리더기를 사용하는 사용자가 오직 귀로만 테이블의 정보를 얻어야 할 경우, 
테이블의 데이타를 인식하고 읽는 순서를 결정하기 때문이다.
웹표준, 접근성을 고려해서 홈페이지를 제작 한다면 반드시 준수해야 할 사항이다.<br><br>

복잡한 구조의 테이타 테이블<br>
<table width="100%" summary="데이타테이블 설명" class="datatable">
<caption>표제목</caption>
<thead>
  <tr>
    <th rowspan="2" scope="col">전체 구분1 </th>
    <th colspan="3" scope="colgroup">구분 1 </th>
  </tr>
  <tr>
    <th scope="col">구분 1-1 </th>
    <th scope="col"> 구분 1-2 </th>
    <th scope="col">구분1-3</th>    
  </tr>
</thead>
<tbody>
  <tr>
    <th scope="row">구분 A</th>
    <td>내용 1-1-A</td>
    <td>내용 1-2-A</td>
    <td>내용 1-3-A</td>
  </tr>
  <tr>
    <th scope="row">구분 B</th>
    <td>내용 1-1-B</td>
    <td>내용 1-2-B</td>
    <td>내용 1-3-B</td>
  </tr>
  <tr>
    <th scope="row">구분 C</th>
    <td>내용 1-1-C</td>
    <td>내용 1-2-C</td>
    <td>내용 1-3-C</td>
  </tr>
</tbody>
</table>

{% highlight html %}
<table width="100%" summary="데이타테이블 설명" class="datatable">
<caption>표제목</caption>
<thead>
  <tr>
    <th rowspan="2" scope="col">전체 구분1 </th>
    <th colspan="3" scope="colgroup">구분 1 </th>
  </tr>
  <tr>
    <th scope="col">구분 1-1 </th>
    <th scope="col"> 구분 1-2 </th>
    <th scope="col">구분1-3</th>    
  </tr>
</thead>
<tbody>
  <tr>
    <th scope="row">구분 A</th>
    <td>내용 1-1-A</td>
    <td>내용 1-2-A</td>
    <td>내용 1-3-A</td>
  </tr>
  <tr>
    <th scope="row">구분 B</th>
    <td>내용 1-1-B</td>
    <td>내용 1-2-B</td>
    <td>내용 1-3-B</td>
  </tr>
  <tr>
    <th scope="row">구분 C</th>
    <td>내용 1-1-C</td>
    <td>내용 1-2-C</td>
    <td>내용 1-3-C</td>
  </tr>
</tbody>
</table>
{% endhighlight %}

구분 1에는 scope="colgroup" 를 넣어줘야 한다. <br>
만약 구분1 처럼 병합셀이 행이 아닌 열에 있다면 반대로 scope="rowgroup" 이라고 표시하면 된다. <br>
