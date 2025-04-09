# Pict



@model IEnumerable<BookDetails>

<h2>Book List</h2>

<table id="getBooks" border="1">
    <thead>
        <tr>
            <th>Id</th>
            <th>Title</th>
            <th>Author</th>
            <th>Genre</th>
            <th>Total Copies</th>
            <th>Available Copies</th>
            <th>Branch</th>
        </tr>
    </thead>
    <tbody>
        @foreach (var book in Model)
        {
            <tr>
                <td>@book.Id</td>
                <td>@book.Title</td>
                <td>@book.Author</td>
                <td>@book.Genre</td>
                <td>@book.TotalCopies</td>
                <td>@book.AvailableCopies</td>
                <td>@book.Branch?.BranchName</td>
            </tr>
        }
    </tbody>
</table>
