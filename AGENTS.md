<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

- Brand info, categories and image imports live in `src/lib/site.ts`; pages read from it so photos/contact details can be swapped in one place.
- Enquiries go through the `submitEnquiry` server function into the `enquiry_submissions` table (insert-only for visitors) so submissions are validated server-side and never read publicly.
