# Formik With Tanstack Query 4

## Notes

- when using an async submit handler, need to explicitly call `setSubmitting(false)`; this is not the case when using non-async submit handler

https://formik.org/docs/api/formik#onsubmit-values-values-formikbag-formikbag--void--promiseany

> IMPORTANT: If onSubmit is async, then Formik will automatically set isSubmitting to false on your behalf once it has resolved. This means you do NOT need to call formikBag.setSubmitting(false) manually. However, if your onSubmit function is synchronous, then you need to call setSubmitting(false) on your own.

https://formik.org/docs/api/formik#setsubmitting-issubmitting-boolean--void

> `setSubmitting: (isSubmitting: boolean) => void`
>
> Set isSubmitting imperatively. You would call it with setSubmitting(false) in your onSubmit handler to finish the cycle. To learn more about the submission process, see Form Submission.

https://formik.org/docs/guides/form-submission#submission

> **Submission**
> 
> Proceed with running your submission handler (i.e.onSubmit or handleSubmit)
> you call setSubmitting(false) in your handler to finish the cycle


