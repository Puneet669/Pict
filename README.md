# Pict



@model IEnumerable<BranchDetails>

<h2>Branch List</h2>

<table id="getBranches" border="1">
    <thead>
        <tr>
            <th>Branch Id</th>
            <th>Name</th>
            <th>Location</th>
            <th>City</th>
        </tr>
    </thead>
    <tbody>
        @foreach (var branch in Model)
        {
            <tr>
                <td>@branch.BranchId</td>
                <td>@branch.BranchName</td>
                <td>@branch.BranchLocation</td>
                <td>@branch.City</td>
            </tr>
        }
    </tbody>
</table>
