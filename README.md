# Free HTML form templates

21 copy-and-paste form templates in plain HTML and Tailwind CSS: contact, newsletter, waitlist, feedback, quote request, job application and more. Accessible markup, real labels, no dependencies.

Each form is ready to send to [FormTango](https://formtango.com), a form backend: submissions are stored in an inbox, checked for spam and emailed to you, with no server code.

## Templates

| Template | What it is | Fields | Files |
| --- | --- | --- | --- |
| [Contact form](./contact-form/index.html) | Name, email and a message. The form every website needs. | 3 | [HTML](./contact-form/index.html) · [Tailwind](./contact-form/tailwind.html) |
| [Newsletter signup](./newsletter-signup/index.html) | One email field and a button. | 1 | [HTML](./newsletter-signup/index.html) · [Tailwind](./newsletter-signup/tailwind.html) |
| [Waitlist](./waitlist/index.html) | Collect interest before you launch. | 2 | [HTML](./waitlist/index.html) · [Tailwind](./waitlist/tailwind.html) |
| [Feedback form](./feedback-form/index.html) | A rating and a comment. | 3 | [HTML](./feedback-form/index.html) · [Tailwind](./feedback-form/tailwind.html) |
| [Quote request](./quote-request/index.html) | For freelancers, agencies and trades. | 6 | [HTML](./quote-request/index.html) · [Tailwind](./quote-request/tailwind.html) |
| [Job application](./job-application/index.html) | Contact details, a cover note and a CV upload. | 7 | [HTML](./job-application/index.html) · [Tailwind](./job-application/tailwind.html) |
| [Event RSVP](./event-rsvp/index.html) | Who is coming, and how many. | 5 | [HTML](./event-rsvp/index.html) · [Tailwind](./event-rsvp/tailwind.html) |
| [Booking request](./booking-request/index.html) | A preferred date and what the booking is for. | 5 | [HTML](./booking-request/index.html) · [Tailwind](./booking-request/tailwind.html) |
| [Support request](./support-request/index.html) | A topic, a description and an optional screenshot. | 4 | [HTML](./support-request/index.html) · [Tailwind](./support-request/tailwind.html) |
| [Bug report](./bug-report/index.html) | What happened, what was expected, and where. | 5 | [HTML](./bug-report/index.html) · [Tailwind](./bug-report/tailwind.html) |
| [Callback request](./callback-request/index.html) | A name, a number and the best time to call. | 3 | [HTML](./callback-request/index.html) · [Tailwind](./callback-request/tailwind.html) |
| [Volunteer signup](./volunteer-signup/index.html) | For charities, clubs and community groups. | 6 | [HTML](./volunteer-signup/index.html) · [Tailwind](./volunteer-signup/tailwind.html) |
| [Event registration form](./event-registration/index.html) | Sign people up for a workshop, class, meetup or conference. | 6 | [HTML](./event-registration/index.html) · [Tailwind](./event-registration/tailwind.html) |
| [Order form](./order-form/index.html) | Take simple orders or order enquiries without a shop. | 7 | [HTML](./order-form/index.html) · [Tailwind](./order-form/tailwind.html) |
| [Survey form](./survey/index.html) | A short customer survey with a score and open questions. | 4 | [HTML](./survey/index.html) · [Tailwind](./survey/tailwind.html) |
| [Client intake form](./client-intake/index.html) | Gather what you need before a first meeting. | 8 | [HTML](./client-intake/index.html) · [Tailwind](./client-intake/tailwind.html) |
| [Demo request form](./demo-request/index.html) | Let prospects book a product demo. | 5 | [HTML](./demo-request/index.html) · [Tailwind](./demo-request/tailwind.html) |
| [Rental application form](./rental-application/index.html) | Collect applications for a property to let. | 9 | [HTML](./rental-application/index.html) · [Tailwind](./rental-application/tailwind.html) |
| [File upload form](./file-upload-form/index.html) | A contact form that accepts an attachment. | 4 | [HTML](./file-upload-form/index.html) · [Tailwind](./file-upload-form/tailwind.html) |
| [Simple contact form](./simple-contact-form/index.html) | Just an email address and a message. | 2 | [HTML](./simple-contact-form/index.html) · [Tailwind](./simple-contact-form/tailwind.html) |
| [Lead capture form](./lead-capture-form/index.html) | Name, work email, company and what they need. | 4 | [HTML](./lead-capture-form/index.html) · [Tailwind](./lead-capture-form/tailwind.html) |

## Use one

1. Open a template's `index.html` (plain HTML with a little CSS) or `tailwind.html`.
2. Copy the `<form>` into your page.
3. Replace `YOUR_FORM_ID` with your form's id.

### Get a form id

Sign up free at https://formtango.com (100 submissions a month), or create a form with no account:

```bash
curl -X POST https://formtango.com/api/v1/claims \
  -H "Content-Type: application/json" -d '{"name":"Contact form"}'
```

The response has the `endpoint` to use and a `claimUrl` to open to see your submissions.

## Notes

- Every field has a `name`, because browsers only send named fields.
- The hidden `_gotcha` field is a spam trap. Leave it in, hidden and empty.
- Forms with a file input use `enctype="multipart/form-data"`. File uploads need a paid FormTango plan.
- Want a different set of fields? Build your own with the [HTML form generator](https://formtango.com/tools/html-form-generator).

Browse these with live previews at https://formtango.com/templates.

## License

MIT. Use them anywhere, with or without FormTango.
