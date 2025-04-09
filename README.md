# Pict



@model IEnumerable<Librarian>

<h2>Librarian List</h2>

<table id="getLibrarians" border="1">
    <thead>
        <tr>
            <th>Id</th>
            <th>Name</th>
            <th>Gender</th>
            <th>Experience</th>
            <th>Contact</th>
            <th>Branch</th>
        </tr>
    </thead>
    <tbody>
        @foreach (var librarian in Model)
        {
            <tr>
                <td>@librarian.Id</td>
                <td>@librarian.Name</td>
                <td>@librarian.Gender</td>
                <td>@librarian.Experience</td>
                <td>@librarian.Contact</td>
                <td>@librarian.Branch?.BranchName</td>
            </tr>
        }
    </tbody>
</table>
