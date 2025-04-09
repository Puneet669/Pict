# Pict



@model BookDetails

<h2>Create Book</h2>

@if (ViewBag.Message != null)
{
    <h2 id="Message">@ViewBag.Message</h2>
}

<form asp-action="CreateBooksDetails" method="post">
    <div><label>Title</label><input asp-for="Title" /><span asp-validation-for="Title"></span></div>
    <div><label>Author</label><input asp-for="Author" /><span asp-validation-for="Author"></span></div>
    <div><label>Genre</label><input asp-for="Genre" /><span asp-validation-for="Genre"></span></div>
    <div><label>Total Copies</label><input asp-for="TotalCopies" /><span asp-validation-for="TotalCopies"></span></div>
    <div><label>Available Copies</label><input asp-for="AvailableCopies" /><span asp-validation-for="AvailableCopies"></span></div>
    <div>
        <label>Branch</label>
        <select asp-for="BranchId" asp-items="Model.Branches"></select>
        <span asp-validation-for="BranchId"></span>
    </div>
    <button type="submit" id="BookCreationBtn">Create</button>
</form>
