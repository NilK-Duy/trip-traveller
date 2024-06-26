_Thẻ a_: Là thẻ inline, chắc chắn là dùng cho liên kết, nó có 3 thuộc tính hay dùng `href`, `target`, và `rel`

- Khi dùng `target` có giá trị là `_blank` thì thẻ a nên thêm thuộc tính `rel="noopener noreferrer"`

- _margin_ : Có thể dùng số âm, có giá trị auto

- _padding_ : Không thể dùng số âm

_text-decoration_: Gạch dưới của thẻ a, `none`, `underline`, `overline`, `line-through`

_line-height_: Khoảng cách giữa các dòng

- Khi những thẻ inline nằm cách nhau thì nó sẽ nằm trên 1 hàng, ngược lại những thẻ block thì nó sẽ tạo ra hàng mới

- _display_: block, inline, inline-block, none, flex, grid

- `block` : Biến thành thẻ block

- `inline` : Biến thành thẻ inline, nó sẽ bị hạn chế vài thuộc tính CSS liên quan tới box-sizing như là padding-top, padding-bottom, margin-top, margin-bottom

- `inline-block` : Biến thành thẻ inline-block, là sự kết hợp giữa inline-block nó sẽ kế thừa đặc tính của inline tức là nằm cạnh nhau thì sẽ nằm trên 1 hàng, có độ rộng bằng nội dung mà nó chứa, không bị hạn chế CSS

- `none` : Ẩn luôn, không thấy không nhấn được

- `flex` : Dùng rất nhiều hiện nay, nếu master được nó thì code layout vô tư

- _min-width_ : Độ rộng tối thiểu, ví dụ 100px -> >= 100px

- _max-width_ : Độ dài tối đa, ví dụ 200px -> <= 200px

- _flex-box_ : Áp dụng thuộc tính display: flex vào phần tử mình muốn dàn layout

- _flex-direction_: row, column, row-reverse, column-reverse

- `row`: Flex theo hàng, chiều ngang, còn row-reverse sẽ đảo ngược các phần tử lại

- `column`: Flex theo cột, chiều dọc, còn column-reverse sẽ đảo ngược các phần tử lại

- _align-items_: stretch, flex-start, flex-end, center, baseline

- `stretch` : Mặc định của thuộc tính align-items. Giúp các cột có chiều cao bằng nhau - đối với row, giúp các phần tử có chiều rộng bằng nhau - đối với column

- `flex-start` : Căn phần trên bằng nhau

- `flex-end` : Căn phần dưới bằng nhau

- `center` : Căn giữa với khoảng cách trên dưới bằng nhau

- `baseline` : Căn theo dòng chữ đầu tiên của khối

- _calc_: Hàm dùng để tính toán, + - `*` /, lưu ý là phải có khoảng cách giữa các phép tính

- _component_: Mục đích là tái sử dụng và có thể tùy chỉnh 1 chỗ để sử dụng nhiều nơi

- _justify-content_: flex-start, flex-end, center, space-between, space-around, space-evenly
  (Nên lưu ý dùng có thể có sai số khoảng cách với các margin, padding có trước)

- `flex-start` : các phần tử bắt đầu bằng bên trái

- `flex-end` : các phần tử bắt đầu bằng bên phải

- `center` : các phần tử được căn ra giữa

- `space-between` : căn đều sang hai bên, khoảng cách ở giữa để trống

- `space-around` : căn đều các phần tử với khoảng cách ở giữa gấp đôi khoảng cách bên trái và phải

- `space-evenly` : căn đều các phần tử với khoảng cách bằng nhau

- _column-gap_: Khoảng trống chiều dọc

- _row-gap_: Khoảng trống chiều ngang

- _gap_: column-gap row-gap; //Viết tắt đối với gap

- _position_: có 5 giá trị chính: relative, absolute, static, sticky, fixed. Khi sử dụng thuộc tính position này thì đi kèm sẽ có các thuộc tính khác như top right bottom left z-index

- `relative` : Khi sử dụng giá trị này thì phải lưu ý xem phần tử con của nó có sử dụng position là `absolute` không

- `absolute` : Khi sử dụng giá trị này thì phải lưu ý xem phần tử chứa nó có gần nhất có sử dụng _position_ là `absolute` hay `relative` không ?

- _reponsive_:
- _breakpoints_: 320px 480px 768px 1024px 1200px 1366px 1440px 1600px 1920px
- _min-width_: breakpoints
- _max-width_: breakpoints - 0.02px
- _media queries_:
  <!--
  @media screen and (min-width: breakpoints)
  @media screen and (min-width: 320px){}
  -->

  <!--
  @media screen and (max-width: breakpoints -0.02px)
  @media screen and (max-width: 1023.98px){}
  -->

  <!-- @media screen and (min-width: breakpoints) and (max-width: breakpooints){} -->

- _transform_: translate(translateX, translateY), skew(skewX, skewY), rotate(rotateX,Y,Z), scale(X, Y)
- `translateX` : Nếu giá trị là số dương thì nó sẽ di chuyển qua bên phải, ngược lại thì di chuyển qua bên trái
- `translateY` : Nếu giá trị là số dương thì nó đi xuống, ngược lại nó sẽ đi lên
- `value` : 10px, 20px, -15px, -30px, 10%, lưu ý khi sử dụng % thì % ở đây chính là độ rộng hoặc chiều cao của khối chúng ta đang áp dụng thuộc tính transform và hàm translate

- _variables_: Biến là gì? Khai báo như thế nào? Cách sử dụng ra sao? Ưu và nhược điểm của nó là gì?
<!-- usage: var(--primary-color) -->

- _grid_: Dàn layout cực nhanh
  <!--
  align-items: start end center baseline stretch
  justify-content: start end center space-between space-around space-evenly
  track-line: 1 -1
  grid-template-columns: value value value ... n-value: px, %, em, rem
  1fr = fraction unit
  -->

  <!-- grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-columns: 200px repeat(2, 1fr) 300px;  -->

  <!-- grid-auto-flow: column;
  grid-auto-columns: 1fr; -->

  <!-- --columns: 4;
  grid-template-columns: repeat(var(--columns), 1fr); -->
