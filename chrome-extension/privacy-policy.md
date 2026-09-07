# Navigo PDF Chrome extension — privacy policy

Effective date: September 7, 2026. Scope: Navigo PDF Chrome extension 1.0.1.

## What Navigo PDF does

Navigo PDF opens and processes PDF documents in Chrome. Viewing, annotations, form filling, page organization, and exports run on your device. There is no Navigo-operated document-upload service in this extension.

Navi AI is optional. It sends your PDF and conversation to Google Gemini only when you configure an API key and model and submit a message with Send, including the Enter-key shortcut shown in the composer. Opening the Navi panel or choosing a suggested question alone does not upload the PDF.

## Documents and edits

Navigo reads PDF data you open from a website, choose from your computer, or drag into the viewer. This can include page text and images, annotations, form values, attachments, document metadata, and any personal or sensitive information within the PDF. It uses that data to display the PDF and perform the document actions you choose.

Open document bytes, edits, undo history, and comparison documents are held in the viewer session. Saving or exporting creates a download to the location managed by your browser. The extension does not automatically replace the original local file or save a copy to a Navigo cloud account. Closing the viewer discards unsaved application state; your downloaded files remain where you saved them.

If you choose Read aloud, PDF text is passed to the speech-synthesis service supplied by your browser or operating system. Available voices and their handling are controlled by that service; this policy does not promise that every system voice is processed locally.

## Remote PDF addresses and browser navigation

For a remote PDF, Navigo requests the document directly from the original server. The server receives the normal connection/request information, including the source URL, your network address, and credentials that Chrome permits for that request. Navigo does not read stored cookies through a cookies API. HTTP links use the source's HTTP connection; HTTPS links use HTTPS.

To open PDF links automatically and preserve page fragments such as #page=7, the extension observes top-level HTTP, HTTPS, and permitted file navigations. It keeps the latest eligible URL for each tab in local session storage. That value may be a non-PDF page address, and navigation capture continues when automatic PDF opening is off. Later eligible navigation replaces it; closing the tab removes it. This storage is not a cumulative browsing-history log and is not uploaded by the extension.

The original PDF address, including its query parameters and page fragment, appears inside the Navigo viewer URL. An “Open original PDF” exception also holds that exact source address in a tab-scoped rule for the browser session or until the tab is closed/reopened through the Navigo toolbar. Chrome may retain addresses in its own history, session restore, or bookmarks according to your browser settings.

Website permissions let Navigo open PDFs from arbitrary hosts, including URLs without .pdf in the path. The extension does not inject content scripts into arbitrary webpages, enumerate your local directories, or operate an advertising or browsing-analytics service. Local file URL access additionally requires Chrome's “Allow access to file URLs” switch; selecting a file through the viewer is a separate user action.

## Preferences and recent filenames

The extension saves the automatic-opening preference in local Chrome extension storage. The viewer stores recent PDF filenames, favorite filenames, and default zoom in extension-origin localStorage. Recent filenames help you identify documents to choose again; they are not stored copies of those PDFs. The implementation does not synchronize these values through a Navigo account or Chrome sync storage.

Local preferences remain until changed or cleared through Chrome's extension data controls/removal. The current API key and Gemini model setting are held in memory, not written to persistent extension storage.

## Optional Google Gemini requests

When you send a Navi message, Navigo sends the full current PDF, your prompt, and the conversation history to Google's Gemini API over HTTPS at generativelanguage.googleapis.com. It sends your API key to Google as an authentication header. Replies are displayed in Navi. If you enable “Use web + general knowledge,” the request asks Google to use its Google Search tool as part of answering.

The composer and settings disclose the PDF/chat transfer before sending. The AI feature is not required to view or edit PDFs. Your key and chat are held in the current viewer session, and closing that session clears the extension's in-memory copy. Clearing local state does not recall data already transmitted to Google.

Google processes these requests under its [Gemini API terms](https://ai.google.dev/gemini-api/terms) and applicable Google policies. Data treatment depends on the API project, billing status, region, and other applicable terms. This policy does not promise that Google never retains requests, uses them for model/product improvement, or permits human review. Review the terms for your project before sending information. Provider charges may apply to your API project.

## Other recipients and tracking

The recipients used by the implementation are the PDF's original server when opening a remote address, Google when you explicitly use Navi, and your browser/operating-system services when you request actions such as downloads, printing, or speech. The extension includes no analytics beacons or advertising trackers and does not route PDF or chat requests through a Navigo-operated server.

The Chrome Web Store, Chrome itself, PDF servers, and Google have their own data practices. Those services are distinct from the extension's local state.

## Your choices

- Turn automatic PDF opening off in the toolbar popup or extension settings.
- Grant or remove local file URL access in Chrome's extension Details.
- Use viewing/editing tools without configuring Navi AI.
- Remove the API key from Navi settings or close the viewer session.
- Close document tabs and the viewer to discard unsaved session data.
- Remove the extension or use Chrome's data controls to clear persistent local extension data. Separately remove downloaded files or browser history if desired.

## Limited Use

Navigo PDF uses and transfers user data only to provide the PDF workspace and the optional AI operation you request, as described in this policy. Navigo PDF's use and transfer of information received through Chrome APIs follows the Chrome Web Store User Data Policy, including its Limited Use requirements. Navigo does not use this information for advertising, sale of data, or credit decisions.

Google's separate handling of an API request is described in the Google Gemini section above. The Limited Use statement about Navigo is not a promise that Google never retains, reviews, or uses API data for product improvement; review the Google terms that apply to your project before choosing to send.

## Contact

Privacy and support questions: [amanuelsolomonbbdsa@gmail.com](mailto:amanuelsolomonbbdsa@gmail.com).

This policy should be updated if the extension's data practices change.
