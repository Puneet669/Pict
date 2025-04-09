# Pict


@model IEnumerable<Members>

<h2>Member List</h2>

<table id="getMembers" border="1">
    <thead>
        <tr>
            <th>Id</th>
            <th>Name</th>
            <th>Gender</th>
            <th>Contact</th>
            <th>Branch</th>
        </tr>
    </thead>
    <tbody>
        @foreach (var member in Model)
        {
            <tr>
                <td>@member.Id</td>
                <td>@member.Name</td>
                <td>@member.Gender</td>
                <td>@member.Contact</td>
                <td>@member.Branch?.BranchName</td>
            </tr>
        }
    </tbody>
</table>
