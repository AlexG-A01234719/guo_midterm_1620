# Short Answer questions

Alex Guo
A01234719
midterm for 1620 October 2020
BCIT

## Q1
Git is a version control system that allows the user to manage and keep track of source code history.
Git Hub is not the same as Git, it is a cloud-based hosting service that allows the user to manage Git repositories.

## Q2
A branch in Git is a lightweight movable pointer for commits made. The "*lightweight*" means light in terms of data it carries and the little mess it creates. 
Similar to a branch of a tree. The tree branch is attached to part of the main body of the tree trunk. Therefore, while branches continue to grow and fall.
The tree is still considered alive so long as the trunk remains standing.
To create a branch using Git, simply entering `git branch {branch_name}` will create a new branch named "branch_name" in your repository.

## Q3
The status code for **not found** is 404, and it is a client error response. This reponse is a perment representation of the error because it means that the
server cannot find the requested resource from the URL provided, which implies that the resource itself does not exist anymore.

## Q4
The styling for h2 is incorrect and will not be applied because the h2 element is assigned to an id called "school" (does not really matter in this case for this question), and it has an inline style element giving it `"color: red;"`. Because the inline css has the highest priority, the h2 color will be red.

## Q5
Example URL: `https://www.example.com:1234/path/file.html?key1=value1&key2=value2#SomewhereInTheDocument`
- `https` is the protocol, and it is the first part of the URL indicating which protocol the browser must use.
- `www.example.com` is the domain name, and it indicates which web server is being requested.
- `:1234` is the port, and it indicates the technical gate used to access resources on the web server. Usually omitted if standard ports are used.
- `/path/file.html` is the path to the resource on the web server.
- `?key1=value1&key2=value2` are extra parameters provided to the web server.
- `#SomewhereInTheDocument` is an anchor to another part of the resource itself, acting as a sort of "bookmark" inside the resource, providing instructions to the browser to show content at the "bookmarked" location.

## Q6
HTTP headers are used to pass through additional information between the clients and the server using an HTTP request or response.
<br />Example headers:
- `Device-Memory` represents an approximate mount of RAM the client has.
- `Last-Modified` shows the last modification date of the resource, used to compare different versions of the same resource.
- `DNT` indicates the user's tracking preferences.

## Q7
The CSS box model is essentially a box that wraps around every HTML element, and consists of the following parts:
- Content - The content of the box, where text and images appear.
- Padding - Clears an area around the content. The padding is transparent.
- Border - A border that goes around the padding and content.
- Margin - Clears an area outside the border. The margin is transparent.

## Q8
- **Descendant combinator** combines two selectors so that elements matched by the second selector are selected if they have an ancestor element matching the first selector.
e.g. `.class p {color: red;}` Selects `p` if it is in class named `class`.
- **Child combinator** matches only elements matched by the second selector that are direct children of elements matched by the first. 
e.g. `ul > li {border: 5px solid blue;}` Selects only `li` under `ul`.
- **Adjacent sibling combinator** is used to select something if it is right next to another elment at the same level of hierarchy.
e.g. `h1 + p {font-weight: bold;}` Selects only the `p` right next to `h1`, and will not work if there is anything else other than a `p` under `h1` in the HTML.
- **General sibling combinator** Selects siblings of an element even if they are not directly adjacent.
e.g. `h1 ~ p {background-color: #777;}` Selects all `p` elements that come after `h`.

## Q9
These two paragraphs will appear on two separate lines because the `p` tag always starts the paragraph on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.

## Q10
There is an error with the `img` tag and `a` tag. The `img` is missing an `alt` alternate text for the image used for if the image cannot be displayed (which is the case here).
The `a` is not closed properly formatted at the middle where there is an extra `<`, and at the end with `</a>`, instead it has `/a>`. That is it for technical issues, but then displaying `title="bcit"` does not make sense here, so that should also be removed to only say `bcit site`.