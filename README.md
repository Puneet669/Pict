# Pict


@model BranchDetails

<h2>Create Branch</h2>

@if (ViewBag.Message != null)
{
    <h2 id="Message">@ViewBag.Message</h2>
}

<form asp-action="Create" method="post">
    <div>
        <label>Branch Name</label>
        <input asp-for="BranchName" />
        <span asp-validation-for="BranchName"></span>
    </div>
    <div>
        <label>Branch Location</label>
        <input asp-for="BranchLocation" />
        <span asp-validation-for="BranchLocation"></span>
    </div>
    <div>
        <label>City</label>
        <input asp-for="City" />
        <span asp-validation-for="City"></span>
    </div>
    <button type="submit" id="BranchCreationBtn">Create</button>
</form>
